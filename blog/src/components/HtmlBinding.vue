<template>
    <div>
        <h1>HTML Binding</h1>
        <p>{{ name }}</p>
       <div v-html="tag1"></div>
       <div v-html="tag2"></div>
    </div>
</template>
<script>
export default{
    name: "HtmlBinding",
    data(){
        return{
            name : "kirti",
            tag1 : "<h1>hello kirti</h1>",
            tag2:"<h2>Age is 21</h2>"
        }
    }
}
</script>