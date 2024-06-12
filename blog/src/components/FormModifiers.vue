<template>
<div>
    <h1>Form Modifiers</h1>
    <input type = "number" v-model.lazy.number="name" placeholder="Enter Your Name"/>
    <p>Name : {{ name }} {{ typeof(name) }}</p>
</div>
</template>
<script>
export default {
    name : "FormModifiers",
    data(){
        return{
            name : ""
        }

    }
}
</script>