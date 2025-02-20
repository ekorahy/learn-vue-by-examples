<script setup>
import { ref } from 'vue'

const text = ref('Edit me')
const checked = ref(true)
const checkedNames = ref(['Jack'])
const picked = ref('One')
const selected = ref('A')
const multiSelected = ref(['A'])
</script>

<template>
  <section>
    <h3>Text Input</h3>
    <input type="text" v-model="text" />
    <p>{{ text }}</p>

    <h3>Checkbox</h3>
    <input type="checkbox" id="checkbox" v-model="checked" />
    <label for="checkbox">Checked: {{ checked }}</label>

    <h3>Multi Checkbox</h3>
    <input type="checkbox" id="jack" value="Jack" v-model="checkedNames" />
    <label for="jack">Jack</label>
    <input type="checkbox" id="john" value="John" v-model="checkedNames" />
    <label for="john">John</label>
    <input type="checkbox" id="mike" value="Mike" v-model="checkedNames" />
    <label for="mike">Mike</label>
    <p>Checked names: {{ checkedNames }}</p>

    <h3>Radio</h3>
    <input type="radio" id="one" value="One" v-model="picked" />
    <label for="one">One</label>
    <br />
    <input type="radio" value="Two" id="two" v-model="picked" />
    <label for="two">Two</label>
    <p>Picked: {{ picked }}</p>

    <h3>Select</h3>
    <select v-model="selected">
      <option disabled value="">Please select one</option>
      <option>A</option>
      <option>B</option>
      <option>C</option>
    </select>
    <p>Selected: {{ selected }}</p>

    <h3>Multi Select</h3>
    <select v-model="multiSelected" multiple style="width: 100px">
      <option>A</option>
      <option>B</option>
      <option>C</option>
    </select>
    <p>Selected: {{ multiSelected }}</p>
  </section>
</template>
