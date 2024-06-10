<template>
    <div>
        <h1>Get Value Input</h1>
        <div> <input type="text" v-model="name" placeholder="Enter your name"></div>
        <div> <input type="text" v-model="email" placeholder="Enter your email"></div>
        <button v-on:click = "GetValues()">Click Me</button>
    </div>
    </template>
    
    <script>
    export default {
        name: 'GetValueInput',
        data(){
            return{
                name : null,
                email : null,
               
            }
        },
        methods:{
            GetValues(){
                    console.log(this.name,this.email)
                }
        }
    }
    </script>
    