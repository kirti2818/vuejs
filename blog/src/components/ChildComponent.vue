<template>
    <div>
        <h2>Child </h2>
        <p>Message :  {{ message }}</p>
        <p>Name : {{ data.name }} , Age : {{ data.age }}</p>
        <button v-on:click="getData()">Click Me</button>
    </div>
</template>
<script>
export default {
    name: "ChildComponent",
    props:{
        message:String,
        data:Object,
        getData:Function
    }

}

</script>