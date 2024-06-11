<template>
    <div>
        <h1>Teacher Component</h1>
        {{ name }}
    </div>
</template>
<script>
export default {
    name: "TeacherComponent",
    props:{
        name:String
    }
}
</script>