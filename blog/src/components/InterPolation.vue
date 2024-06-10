<template>
    <div>
     <h1> Interpolation</h1>
     <p> {{ 10 + 10 }}</p>
     <p>name : {{ name }}</p>
     <p>{{ name = "gupta"}}</p>   
    </div>
</template>
<script>
export default{
    name : 'InterPolation',
    data(){
        return{
            name : "kirti"
        }
    }
}
</script>