<script>
import { ref } from 'vue';

export default{
    data(){
        return{
          items:([
         'HOME',
         'ABOUT',
         'PROJECTS',
         'PROJECTS',
         'CONSULTATION',
         'CONTACT',
        ])
        }
    }
}
</script>

<template>
         <header class="max-w-[1200px] mx-auto">
            <div class="flex items-center justify-between  py-[39px]">
                <div class="flex items-center justify-between gap-[61px]">
                    <div class=" bg-[#377DFF] w-[40px] h-[40px] rounded-[50%] flex justify-center items-center text-white">D</div>

                    <ul class="flex gap-[40px]">
                    <li class="list-none font-[500]" v-for="item in items">{{item}}</li>
                    </ul>

                </div>
                <div class="flex gap-[40px]">
                    <img src="../assets/img/icon_twitter.svg" alt="icon_twitter">
                    <img src="../assets/img/icon_instagram.svg" alt="icon_instagram">
                    <img src="../assets/img/icon_dribbble.svg" alt="icon_dribbble">
                    <img src="../assets/img/icon_medium.svg" alt="icon_medium">
                </div>
            </div>
    </header>
</template>