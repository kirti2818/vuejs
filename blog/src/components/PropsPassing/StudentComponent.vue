<template>
    <div>
        <h2>Student Component</h2>
        <p>{{ name }}</p>
    </div>
</template>
<script>
export default {
    name: "StudentComponent",
    props:{
        name:String
    }
}
</script>