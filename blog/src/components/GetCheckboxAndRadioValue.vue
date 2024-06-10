<template>
<div>
    <h1>Get Checkbox And Radio Value</h1>
  <div>
    <h2> Specification</h2>
    <label for="developer"> Developer</label>
    <input v-model="Specification" type="checkbox" value = "developer" id="developer"/>

    <label for="student"> Student</label>
    <input v-model="Specification" type="checkbox" value="student" id = "student"/>
  </div>
  <h2>{{ Specification }}</h2>

  <div>
    <h2> Programming Language</h2>
    <label for="java"> Java</label>
    <input v-model="language" type="radio"  value = "java" id="java"/>

    <label for="php"> Php</label>
    <input v-model="language" type="radio"  value="php" id = "php"/>

    <label for="node"> Node</label>
    <input  v-model="language" type="radio"   value="node" id = "node"/>
  </div>
  <h2>{{ language }}</h2>
</div>
</template>
<script>
export default {
    name: 'GetCheckboxAndRadioValue',
    data(){
        return{
         Specification : [],
         language:null
        }
    }
}
</script>