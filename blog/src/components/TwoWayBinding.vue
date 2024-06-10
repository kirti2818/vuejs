<template>
    <div>
        <h1>Two Way Binding</h1>
        <input type="text" v-model="name" placeholder="Enter your name">
        <p>Your name is : {{ name }}</p>
    </div>
</template>
<script>
export default {
    name : 'TwoWayBinding',
    data(){
        return{ 
            name : "Kirti Gupta"
        }
    }
}
</script>