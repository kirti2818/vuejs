<template>
    <div>
  <ul><li v-for="item in error" v-bind:key="item">{{ item }} is not valid</li></ul>
        <h1>Form With Validation</h1>
        <div>
            <label >Email : </label>
            <input type = "text" placeholder="Enter your email" v-model="form.email"/>
        </div>
        <br/> <br/>
        <div>
            <label >Password : </label>
            <input type = "password" placeholder="Enter your Password" v-model="form.password"/>
        </div>
        <br/> <br/>
        <div>
           <h3>Country</h3>
            <select v-model="form.country">
                <option value="in">India</option>
                <option value="usa">USA</option>
                <option value="ch">China</option>
            </select>
        </div>
        <br/> <br/>
        <div >
            <h3>Gender</h3>
           <label for="male">Male</label>
           <input type="radio" value="male" id="male" v-model="form.gender"/>
           <label for="female">Female</label>
           <input type="radio" value="female" id="female" v-model="form.gender"/>
           <label for="other">Other</label>
           <input type="radio" value="other" id="other" v-model="form.gender"/>

        </div>
        <br/> <br/>

        <div>
            <h3>Technology</h3>
           <label for="java">Java</label>
           <input type="checkbox" value="java" id="java" v-model="form.technology"/>
           <label for="node">Node</label>
           <input type="checkbox" value="node" id="node" v-model="form.technology"/>
           <label for=".net">.Net</label>
           <input type="checkbox" value=".net" id=".net" v-model="form.technology"/>

        </div>
        <br/> <br/>
        <button v-on:click = "getFormData">Submit</button>

    </div>
</template>
<script>
export default {
    name : "FormWithValidation",
    data(){
        return{
            form:{
                email:"",
                password:"",
                gender:"",
                technology:[],
                country:""
            },
            error:[]
        }
    },
    methods:{
        getFormData(){
            this.error = [];
            const form = this.form;
            for(const item in form){
                if(typeof(form[item])!=="string" && form[item].length === 0){
                    this.error.push(item)
                    continue;
                }
                if(!form[item]){
                    this.error.push(item)
                }
            }
            if(this.error.length === 0){
                alert("Form Submitted Successfully")
            }
            // console.log(this.form,this.error)
        }
    }
}
</script>