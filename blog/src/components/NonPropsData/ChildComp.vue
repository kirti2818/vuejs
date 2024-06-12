<template>
    <div>
        <h1>Child Component</h1>
        <p v-bind="$attrs">Name : {{ name }}</p>
    </div>
</template>
<script>

export default {
    name : "ChildComp",
    inheritAttrs:false,
    props:{
        name : String,
     
    }
}
</script>