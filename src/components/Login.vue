<template>
    <div>
        <h1>Vue Form</h1>
        <input id="myInput" type="username" placeholder="username"  v-model="loginForm.username" /> <br> <br>
        <input id="myInput" type="password" placeholder="password"    v-model="loginForm.password" /> <br> <br> <br>
        <button v-on:click="loginData">Log In</button>
    </div>
</template>

<script>
export default{
    name: 'Login',
    methods:{
        LoginData(){
            console.log("logindata")
        }
    },
    data(){
        return{
            loginForm:{
                username: null,
                password: null,
            }
        }
    }
}
</script>
    
<style>
    #myInput{
        width: 50%;
        height: 20px;
    }
</style>