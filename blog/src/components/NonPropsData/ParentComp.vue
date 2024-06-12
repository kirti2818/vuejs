<template>
    <div>
        <h1>Parent Component</h1>
        <ChildComp id="childcomp" :name ="name" />
    </div>
</template>
<script>
import ChildComp from './ChildComp.vue'
export default {
    name : "ParentComp",
    components:{
        ChildComp 
    },
    data(){
        return{
            name : "Kirti Gupta"
        }
    }
}
</script>