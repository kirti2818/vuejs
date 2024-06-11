<template>
<div>
    <h1>For Loop</h1>
    <ul>
        <li v-for="item in users" v-bind:key="item.name">
            name is : {{ item.name }} , age is : {{ item.age }}

        </li>
    </ul>
</div>
</template>

<script>
export default {
    name: "ForLoop",
    data() {
        return {
            names: ['John', 'Doe', 'Jane', 'Doe'],
            users:[{name : "John",age:"15"},{name : "kirti",age : "21"}]
        }
    }
}
</script>
