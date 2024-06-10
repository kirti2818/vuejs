<template>
    <div>
        <p>HomePage !</p>
        <p>name : {{ getName() }}</p>
        <p>email : {{ email }}</p>
    </div>

</template>

<script>
export default {
    name: 'HomePage',
    data() {
        return {
            name: "kirti",
            email: "kirti@gmail.com",
           
        }
    },
    methods:{
        getName(){
            return this.name;
        }
    }

}
</script>