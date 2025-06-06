<script setup>
import {ref} from 'vue'

const items =ref([
    'Home',
    'Courses',
    'About',
    'Contact',
    'Become an Instructor'
])
</script>


<template>
    <header>
        <div class="flex justify-between items-center bg-black py-[16px] px-[48px]">
            <ul class="flex gap-[24px]">
                <li v-for="item in items" class="text-white text-[14px] font-medium">{{ item }}</li>
            </ul>
            <div class="flex gap-[24px]">
                <button class="text-[#8C94A3] text-[14px] font-normal">USD</button>
                <img src="../assets/img/ChevronDown.svg" alt="ChevronDown">
                <button class="text-[#8C94A3] text-[14px] font-normal">English</button>
                <img src="../assets/img/ChevronDown.svg" alt="ChevronDown">
            </div>
        </div>

        <div class="flex justify-between items-center bg-white py-[24px] px-[48px] ">

            <div class="flex gap-[8px] items-center ">
                <img class="w-[40px] h-[40px]" src="../assets/logo-project.svg" alt="logo-project">
                <h2 class="text-[32px] font-semibold">E-tutor</h2>

                <buttom class="border-[1px] border-[#d3d4daad] w-[200px] h-[48px] flex items-center ps-[18px] ml-[50px] font-normal">
                    Browse</buttom>
                <img class="w-[16px] h-[16px] relative right-[50px]" src="../assets/img/ChevronDown.svg"
                    alt="ChevronDown">

                <img class="w-[16px] h-[16px] relative left-[40px]" src="../assets/img/MagnifyingGlass.svg"
                    alt="MagnifyingGlass">
                <input class="w-[424px] h-[48px] ps-[40px] border-[1px] outline-none border-[#d3d4daad] font-normal" type="text"
                    placeholder="What do you want learn...">
            </div>


            <div class="flex gap-[24px]">
                <img src="../assets/img/Bell.svg" alt="Bell">
                <img src="../assets/img/Heart.svg" alt="Heart">
                <img src="../assets/img/ShoppingCartSimple.svg" alt="ShoppingCartSimple">
                <button class="w-[168px] h-[48px] bg-[#FFEEE8] text-[#FF6636] text-[16px] font-semibold">Create Account</button>
                <button class="w-[100px] h-[48px] bg-[#FF6636] text-[16px] text-white font-semibold">Sign In</button>
            </div>
        </div>

    </header>
</template>