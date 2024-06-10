<template>
    <div>
        <h1>Parent</h1>
        <!-- <ChildComponent :message = "message" :data = "user" :getData = "GetData" /> -->
       <div>
        <h2>User Component</h2>
        <ul>
        <li v-for="item in usersData" :key="item">
            <UserComponent :data="item" :getName = "GetName"/>
        </li>
       </ul>
       </div>
    </div>
</template>
<script>
//  import ChildComponent from './ChildComponent.vue'
import UserComponent from './UserComponent.vue';
export default {

    name: "ParentComponent",
    components:{
        // ChildComponent,
        UserComponent
    },
    data(){
        return{
            message : "Hello Child",
            user : {name : "John" , age : 15},
            usersData:[{name : "John",age:"15"},{name : "kirti",age : "21"}]
        }
    },
    methods:{
        GetData(){
            alert("Hello I am alert")
        },
        GetName(name){
            alert(`Hello ${name}`)
        }
    }

}

</script>