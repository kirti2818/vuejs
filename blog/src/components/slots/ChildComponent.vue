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
       

    </div>
    </template>
    <script>
  
    export default {
        name : "ChildComponent",
        props:{
            name : String
        }
      
    }
    </script>