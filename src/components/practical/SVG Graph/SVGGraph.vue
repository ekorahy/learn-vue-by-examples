<script setup>
import { ref, reactive } from 'vue'
import PolyGraph from './PolyGraph.vue'

const newLabel = ref('')
const stats = reactive([
  { label: 'A', value: 100 },
  { label: 'B', value: 100 },
  { label: 'C', value: 100 },
  { label: 'D', value: 100 },
  { label: 'E', value: 100 },
  { label: 'F', value: 100 },
])

function add(e) {
  e.preventDefault()
  if (!newLabel.value) return
  stats.push({
    label: newLabel.value,
    value: 100,
  })
  newLabel.value = ''
}

function remove(stat) {
  if (stats.length > 3) {
    stats.splice(stats.indexOf(stat), 1)
  } else {
    alert("Can't delete more!")
  }
}
</script>

<template>
  <div class="graph-container">
    <div>
      <svg width="200" height="200">
        <PolyGraph :stats="stats"></PolyGraph>
      </svg>

      <div v-for="stat in stats" :key="stat">
        <label>{{ stat.label }}</label>
        <input type="range" v-model="stat.value" min="0" max="100" />
        <span>{{ stat.value }}</span>
        <button @click="remove(stat)" class="remove">X</button>
      </div>

      <form id="add">
        <input type="text" name="newLabel" v-model="newLabel" />
        <button @click="add">Add a Stat</button>
      </form>
    </div>

    <pre id="raw">{{ stats }}</pre>
  </div>
</template>

<style>
polygon {
  fill: #43b983;
  opacity: 0.75;
}

circle {
  fill: transparent;
  stroke: #999;
}

text {
  font-size: 10px;
  fill: #666;
}

label {
  display: inline-block;
  margin-left: 10px;
  width: 20px;
}

#raw {
  top: 0;
  left: 300px;
}

.graph-container {
  display: flex;
  gap: 32px;
}
</style>
