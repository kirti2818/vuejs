<template>
    <div>
        <p>Name : {{ data.name }} , Age : {{ data.age }}</p>
        <button v-on:click="getName(data.name)">Alert</button>
    </div>
</template>
<script>
export default{
    name: "UserComponent",
    data(){
        return{
         
        }
    },
    props:{
        data:Object,
        getName:Function
    }
}
</script>