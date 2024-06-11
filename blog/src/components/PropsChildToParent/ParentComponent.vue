<template>
    <div>
        <h1>Parent Component</h1>
        <p v-if="show">Name : {{ data.name }} , Email : {{ data.email }}</p>
        <PropsChildComponent :GetData="GetData"/>
        
    </div>
</template>
<script>
import PropsChildComponent from './ChildComponent.vue'
export default {
    name: "PropsParentComponent",
    components:{
        PropsChildComponent
    },
    data(){
        return{
            show : false,
            data:{}
        }
    },
    methods:{
        GetData(data){
            this.show=!this.show;
            this.data = data;        
        }
    }
}
</script>