<template>
<div>
    <h1>For Loop</h1>
    <ul>
        <l1 v-for="item in users" :key="item.name">
            name is : {{ item.name }} , age is : {{ item.age }}

        </l1>
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
