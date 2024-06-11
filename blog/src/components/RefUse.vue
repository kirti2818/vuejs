<template>
    <div>
        <h1>How to use Ref</h1>
        <input type="text" ref="input" placeholder="Enter your name"  />
        <button v-on:click="RefFunction()">Click Me</button>
    </div>
</template>
<script>
export default{
    name : "RefUse",
    methods:{
        RefFunction(){
            this.$refs.input.focus();
            this.$refs.input.style.color = "red";
            let value = this.$refs.input.value;
            console.log(value)
        }
    }
}
</script>