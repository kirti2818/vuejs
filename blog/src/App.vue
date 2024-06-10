<template>
  <div id="app">
  
    <!-- <HelloWorld msg="Welcome Vue js "/> -->
    <!-- <HomePage /> -->
    <!-- <InterPolation/> -->
    <!-- <MethodsWithParams/> -->
    <!-- <ClickEvent/> -->
    <!-- <TwoWayBinding/> -->
    <!-- <GetValueInput/> -->
    <!-- <GetCheckboxAndRadioValue/> -->
    <!-- <IfElseCondition/> -->
    <!-- <ForLoop/> -->
    <ParentComponent/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import HomePage from './components/HomePage.vue'
// import InterPolation from './components/InterPolation.vue'
// import MethodsWithParams from './components/MethodsWithParams.vue'
// import ClickEvent from './components/ClickEvent.vue'
// import TwoWayBinding from './components/TwoWayBinding.vue'
// import GetValueInput from './components/GetValueInput.vue'
// import GetCheckboxAndRadioValue from './components/GetCheckboxAndRadioValue.vue'
// import IfElseCondition from './components/IfElseCondition.vue'
// import ForLoop from './components/ForLoop.vue'
import ParentComponent from './components/ParentComponent.vue'


export default {
  name: 'App',
  components: {
    // HelloWorld,
    // HomePage,
    // InterPolation,
    // MethodsWithParams,
    // ClickEvent,
    // TwoWayBinding,
    // GetValueInput,
    // GetCheckboxAndRadioValue,
    // IfElseCondition,
    // ForLoop,
    ParentComponent,
  
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
