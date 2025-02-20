<script setup>
import CollapsibleSection from './components/CollapsibleSection.vue'
import HelloWorld from './components/basic/HelloWorld.vue'
import HandlingUserInput from './components/basic/HandlingUserInput.vue'
import AttributeBindings from './components/basic/AttributeBindings.vue'
import ConditionalsAndLoops from './components/basic/ConditionalsAndLoops.vue'
import FormBindings from './components/basic/FormBindings.vue'
import SimpleComponent from './components/basic/SimpleComponent.vue'
</script>

<template>
  <h1>Learn Vue.js by examples</h1>
  <CollapsibleSection title="Basic">
    <CollapsibleSection title="Hello World"> <HelloWorld /></CollapsibleSection>
    <CollapsibleSection title="Handling User Input"><HandlingUserInput /></CollapsibleSection>
    <CollapsibleSection title="Attribute Bindings"><AttributeBindings /></CollapsibleSection>
    <CollapsibleSection title="Conditionals and Loops"><ConditionalsAndLoops /></CollapsibleSection>
    <CollapsibleSection title="Form Bindings"><FormBindings /></CollapsibleSection>
    <CollapsibleSection title="Simple Component"><SimpleComponent /></CollapsibleSection>
  </CollapsibleSection>
</template>
