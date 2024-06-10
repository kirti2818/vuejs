<template>
    <div>
        <h1> Methods With Params</h1>
        <p>name : {{ getName("Peter") }}</p>
        <p>Email : {{ getData().email }}</p>
       
    </div>
</template>
<script>
export default {
    name : 'MethodsWithParams',
   methods:{
    getName(data){
        return data;
    },
    getData(){
        return {
            name : "Kirti Gupta",
            email : "kirti@gmail.com"
        }
    }
   }
}
</script>