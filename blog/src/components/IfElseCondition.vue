<template>
   <div>
    <h1>If Else Condition</h1>
    <p v-if="age>=18">Age is 18</p>
    <p v-else> Age is less than 18</p>
    <div>
        <button v-on:click="age=18">Age 18</button>
        <button v-on:click="age=17">Age 17</button>
    </div>
   </div>
</template>
<script>
export default {
    name: 'IfElseCondition',
    data(){
        return{
            age: 17
        }
    }
}
</script>