<script setup>
import CollapsibleSection from './components/CollapsibleSection.vue'

// Basic components
import HelloWorld from './components/basic/HelloWorld.vue'
import HandlingUserInput from './components/basic/HandlingUserInput.vue'
import AttributeBindings from './components/basic/AttributeBindings.vue'
import ConditionalsAndLoops from './components/basic/ConditionalsAndLoops.vue'
import FormBindings from './components/basic/FormBindings.vue'
import SimpleComponent from './components/basic/Simple Component/SimpleComponent.vue'

// Practical components
import MarkdownEditor from './components/practical/MarkdownEditor.vue'
import FetchingData from './components/practical/FetchingData.vue'
import GridWithSortAndFilter from './components/practical/Grid with Sort and Filter/GridWithSortAndFilter.vue'
import TreeView from './components/practical/Tree View/TreeView.vue'
import SVGGraph from './components/practical/SVG Graph/SVGGraph.vue'
import ModalWithTransitions from './components/practical/Modal with Transitions/ModalWithTransitions.vue'
import ListWithTransitions from './components/practical/ListWithTransitions.vue'
import TodoMVC from './components/practical/TodoMVC.vue'

// 7 GUIs
import CounterComponent from './components/7 GUIs/CounterComponent.vue'
import TemperatureConverter from './components/7 GUIs/TemperatureConverter.vue'
import FlightBooker from './components/7 GUIs/FlightBooker.vue'
import TimerComponent from './components/7 GUIs/TimerComponent.vue'
import CRUD from './components/7 GUIs/CRUD.vue'
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
  <CollapsibleSection title="Practical">
    <CollapsibleSection title="Markdown Editor"><MarkdownEditor /></CollapsibleSection>
    <CollapsibleSection title="Feching Data"><FetchingData /></CollapsibleSection>
    <CollapsibleSection title="Grid with Sort and Filter"
      ><GridWithSortAndFilter />
    </CollapsibleSection>
    <CollapsibleSection title="Tree View"><TreeView /></CollapsibleSection>
    <CollapsibleSection title="SVG Graph"><SVGGraph /></CollapsibleSection>
    <CollapsibleSection title="Modal with Transitions"><ModalWithTransitions /></CollapsibleSection>
    <CollapsibleSection title="List with Transitions"><ListWithTransitions /></CollapsibleSection>
    <CollapsibleSection title="TodoMVC"><TodoMVC /></CollapsibleSection>
  </CollapsibleSection>
  <CollapsibleSection title="7 GUIs">
    <CollapsibleSection title="Counter"><CounterComponent /></CollapsibleSection>
    <CollapsibleSection title="Temperature Converter"><TemperatureConverter /></CollapsibleSection>
    <CollapsibleSection title="Flight Booker"><FlightBooker /></CollapsibleSection>
    <CollapsibleSection title="Timer"><TimerComponent /></CollapsibleSection>
    <CollapsibleSection title="CRUD"><CRUD /></CollapsibleSection>
  </CollapsibleSection>
</template>
