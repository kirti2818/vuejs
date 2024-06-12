<template>
<div>
    <h1>Parent Component</h1>
  <ChildComponent><h1>Kirti Gupta</h1></ChildComponent>
  <ChildComponent><h2>Age is 21</h2></ChildComponent>
  <ChildComponent></ChildComponent>
</div>
</template>
<script>
import ChildComponent from './ChildComponent.vue'
export default {
    name : "ParentComponent",
    components:{
        ChildComponent
    }
}
</script>