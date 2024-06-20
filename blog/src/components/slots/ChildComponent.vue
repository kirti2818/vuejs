<template>
    
    <div>
        <!-- <slot><h1>Default</h1></slot> -->
        <header>
          <slot name="header"></slot>
        </header>
        <content>
            <slot name="content"></slot>
        </content>
        <footer>
            <slot name="footer"><button>Click me</button></slot>
        </footer>
        <button v-on:click="gg">send</button>
       

    </div>
    </template>
    <script>
  
    export default {
        name : "ChildComponent",
        props:{
            name : String,
            isbtndisabled : Boolean,
            update: Function
        },
        methods:{
            gg(){
                console.log("hii") 
                this.update(!this.isbtndisabled)       
            }
        }
      
    }
    </script>