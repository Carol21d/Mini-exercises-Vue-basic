<script setup>
import { ref } from 'vue';

function PasswordShow() {
     let password= document.getElementById("password");
     if (password.type == "password") {
        password.type = "text";
        
     }else{
        password.type ="password";
     }
    
}

 



</script>

<template>
    <div class="container text-center input-password">
        <h1 class="my-3">Exercise Input Password</h1>
        <input type="password" name="password" id="password" class="form-control">
        <div class="d-block">
            <span id="show-password" @click="PasswordShow" class="mt-2 btn btn-warning">Show Password</span>
        </div>
    </div>
</template>

<style lang="css" scoped>
    #show-password:hover {
        cursor: pointer;
        user-select: none;
    }
</style>