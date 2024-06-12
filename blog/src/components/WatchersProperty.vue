<template>
    <div>
        <h1>Watchers Property</h1>
        <h2>{{ count }}</h2>
        <button @click="count++">Increment</button>
        <button @click="count--">Decrement</button>
        
    </div>
</template>
<script>
export default {
    name : "WatchersProperty",
    data(){
        return{
            count:0
        }
    },
    watch:{
        count(val,old){
            if(val>5 && old<val){
                alert("Count is greater than 5")
            }
            // if(val>5 ){
            //    this.count = 0;
            // }
            console.log(this.count)
        }
    }
    
}
</script>