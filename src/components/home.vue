
<template>
<h1>Email: {{email}}</h1>
<h2>Mobile: {{mobile = 2356748}}</h2>
<h2>Name: {{getName("test")}}</h2>
<h2>Age: {{getAge(67)}} years</h2>

<Button @click="btnclick("hello world")">Click Me</Button>
</template>

<script>
export default {
  
    // eslint-disable-next-line vue/multi-word-component-names
    name : "Home",
    data(){
        return {
            email:"test@gmail.com",
            mobile:12345678,
            getName(name){
                return name;
            }
        }
    },
    methods:{
        btnclick(data){
            alert(data)
        },
        getAge(age){
            return age;
        },
        getData(){
            return {
                name:"musila",
            email:this.email
            }
        }
    }
}
</script>

<style scoped>
h1{
    font-size: 20px;
    color: blue;
    text-decoration: underline;
}
</style>