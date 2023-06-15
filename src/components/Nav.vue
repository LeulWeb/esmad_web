<script setup>
    import Logo from "../assets/logo.png";
</script>



<template>
    <nav class="w-screen py-2  bg-[#fff] shadow-md">
        <div class="w-11/12 sm:w-10/12 flex justify-between mx-auto">
            <div class="logo w-[30vw] sm:w-[20vw]">
                <img :src="Logo" alt="">
            </div>

            <!-- Links -->
            <div class="flex space-x-7 items-center">
                <a href="#product">Products</a>
                <a href="#team">About Us</a>
            </div>
        </div>
    </nav>
</template>


<style  scoped>
 
</style>