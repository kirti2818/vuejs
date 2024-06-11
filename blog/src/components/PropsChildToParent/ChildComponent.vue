<template>
    <div>
        <h2> Child Component</h2>
        <button v-on:click="GetData(userData)">send data child to parent</button>
    </div>
</template>
<script>
export default {
    name : 'PropsChildComponent',
    props:{
        GetData:Function
    },
    data(){
        return{
            userData : {name : "kirti" , age : "21",email : "kirti@gmail.com"}
        }
    }
}
</script>