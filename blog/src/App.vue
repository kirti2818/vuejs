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
    <!-- <ParentComponent/> -->
    <!-- <HtmlBinding/> -->
    <!-- <TeacherComponent :name = "Teachername"/>
    <StudentComponent :name = "Studentname"/> -->
    <!-- <PropsParentComponent/> -->
    <!-- <RefUse/> -->
    <!-- <FormWithValidation/> -->
    <!-- <FormModifiers/> -->
    <!-- <ParentComp/> -->
    <!-- <ComputedProperty/> -->
    <!-- <WatchersProperty/> -->
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
// import ParentComponent from './components/ParentComponent.vue'
// import HtmlBinding from './components/HtmlBinding.vue'
// import StudentComponent from './components/PropsPassing/StudentComponent.vue'
// import TeacherComponent from './components/PropsPassing/TeacherComponent.vue'
// import PropsParentComponent from './components/PropsChildToParent/ParentComponent.vue'
// import RefUse from './components/RefUse.vue'
// import FormWithValidation from './components/FormWithValidation.vue'
// import FormModifiers from './components/FormModifiers.vue'
// import ParentComp from './components/NonPropsData/ParentComp.vue'
// import ComputedProperty from './components/ComputedProperty.vue'
// import WatchersProperty from './components/WatchersProperty.vue'
import ParentComponent from './components/slots/ParentComponent.vue'


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
    // ParentComponent,
    // HtmlBinding,
    // StudentComponent,
    // TeacherComponent,
    // PropsParentComponent,
    // RefUse,
    // FormWithValidation,
    // FormModifiers,
    // ParentComp,
    // ComputedProperty,
    // WatchersProperty,
    ParentComponent
    
  
  },
  data(){
    return{
      Teachername : "Kirti Gupta",
      Studentname : "John"
    }
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
