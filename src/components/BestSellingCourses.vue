<script setup>
import { ref } from 'vue'

const courses = ref([
    {
        id: 1,
        name: 'DESIGN',
        mony: '$57',
        text: 'Machine Learning A-Z™:Hands-On Python & R In Data...',
        evaluation: '5.0',
        piople: '265.7K',
        students: 'students',
        img: 'Course1.svg'
    },

    {
        id: 2,
        name: 'Developments',
        mony: '$57',
        text: 'The Complete 2021 Web Development Bootcamp',
        evaluation: '5.0',
        piople: '265.7K',
        students: 'students',
        img: 'Course2.svg'

    },

    {
        id: 3,
        name: 'BUSINESS',
        mony: '$57',
        text: 'Learn Python Programming Masterclass',
        evaluation: '5.0',
        piople: '265.7K',
        students: 'students',
        img: 'Course3.svg'
    },

    {
        id: 4,
        name: 'MARKETING',
        mony: '$57',
        text: 'The Complete Digital Marketing Course - 12 Courses in 1',
        evaluation: '5.0',
        piople: '265.7K',
        students: 'students',
        img: 'Course4.svg'  
    },

    {
        id: 5,
        name: 'IT & SOFTWARE',
        mony: '$57',
        text: 'Reiki Level I, II and Master/Teacher Program',
        evaluation: '5.0',
        piople: '265.7K',
        students: 'students',
        img: 'Course5.svg'
    },

        {
        id: 6,
        name: 'Music',
        mony: '$57',
        text: 'The Complete Foundation Stock Trading Course',
        evaluation: '5.0',
        piople: '265.7K',
        students: 'students',
        img: 'Course6.svg'
    },

    {
        id: 7,
        name: 'Marketing',
        mony: '$57',
        text: 'Beginner to Pro in Excel: Financial Modeling and Valuati...',
        evaluation: '5.0',
        piople: '265.7K',
        students: 'students',
        img: 'Course7.svg'

    },

    {
        id: 8,
        name: 'Health & Fitness',
        mony: '$57',
        text: 'The Python Mega Course: Build 10 Real World Applications',
        evaluation: '5.0',
        piople: '265.7K',
        students: 'students',
        img: 'Course8'
    },

    {
        id: 9,
        name: 'Design',
        mony: '$57',
        text: 'Copywriting - Become a Freelance Copywriter, your ow...',
        evaluation: '5.0',
        piople: '265.7K',
        students: 'students',
        img: 'Course9'  
    },

    {
        id: 10,
        name: 'Lifestyle',
        mony: '$57',
        text: 'Google Analytics Certification - Learn How To Pass The Exam',
        evaluation: '5.0',
        piople: '265.7K',
        students: 'students',
        img: 'Course10'
    }
])

</script>


<template>
    <section class="bg-[#ecebeb79]">
        <div class="max-w-[1320px] mx-auto my-0 ">

            <h2 class="text-[40px] text-center pt-[80px] pb-[40px] font-semibold">Best selling courses</h2>
        
            <div class="flex gap-[25px]">

                <div class="w-[244px] h-[333px] bg-white" v-for="course in courses" :key="course.id">
                    <img :src="`../assets/img/${ course.img }`" alt="Course1">
                    <div class="flex justify-between items-center px-[14px] mt-[14px]">
                        <p class="w-[50px] h-[20px] bg-[#FFEEE8] text-[#993D20] text-[10px] text-center font-medium">
                            {{ course.name }}</p>
                        <p class="text-[16px] text-[#FF6636] font-semibold">{{ course.mony }}</p>
                    </div>
                    <p class="text-[14px] learning-[20px] mt-[10px] ml-[14px] font-medium">{{ course.text }}</p>
                    <div class="flex justify-between items-center  px-[14px] pt-[29px]">
                        <div class="w-[41px] h-[20px] flex justify-between items-center">
                            <img src="../assets/img/Star.svg" alt="Star">
                            <p class="text-[14px] text-[#4E5566] font-medium">{{ course.evaluation }}</p>
                        </div>
                        <div class="flex">
                            <p class="text-[14px] text-[#4E5566] font-medium">{{ course.piople }}</p>
                            <p class="text-[14px] text-[#8C94A3]">{{ course.students }}</p>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>
</template>
                 <!-- <div class="w-[244px] h-[333px] bg-white">
                    <img src="../assets/img/Course2.svg" alt="Course1">
                    <div class="flex justify-between items-center px-[14px] mt-[14px]">
                        <p class="w-[94px] h-[20px] bg-[#EBEBFF] text-[#342F98] text-[10px] text-center font-medium">{{ course.name }}</p>
                        <p class="text-[16px] text-[#FF6636] font-semibold">{{ course.mony }}</p>
                    </div>
                    <p class="text-[14px] learning-[20px] mt-[10px] ml-[14px] font-medium">{{ course.text }}</p>
                    <div class="flex justify-between items-center  px-[14px] pt-[29px]">
                        <div class="w-[41px] h-[20px] flex justify-between items-center">
                            <img src="../assets/img/Star.svg" alt="Star">
                            <p class="text-[14px] text-[#4E5566] font-medium">{{ course.evaluation }}</p>
                        </div>
                        <div class="flex">
                            <p class="text-[14px] text-[#4E5566] font-medium">{{ course.piople }}</p>
                            <p class="text-[14px] text-[#8C94A3]"> {{ course.students }}</p>
                        </div>
                    </div>
                </div>


                <div class="w-[244px] h-[333px] bg-white">
                    <img src="../assets/img/Course3.svg" alt="Course1">
                    <div class="flex justify-between items-center px-[14px] mt-[14px]">
                        <p class="w-[62px] h-[20px] bg-[#E1F7E3] text-[#15711F] text-[10px] text-center font-medium">
                            BUSINESS</p>
                        <p class="text-[16px] text-[#FF6636] font-semibold">$57</p>
                    </div>
                    <p class="text-[14px] learning-[20px] mt-[10px] ml-[14px] font-medium">Learn Python Programming
                        <br /> Masterclass
                    </p>
                    <div class="flex justify-between items-center  px-[14px] pt-[29px]">
                        <div class="w-[41px] h-[20px] flex justify-between items-center">
                            <img src="../assets/img/Star.svg" alt="Star">
                            <p class="text-[14px] text-[#4E5566] font-medium">5.0</p>
                        </div>
                        <div class="flex">
                            <p class="text-[14px] text-[#4E5566] font-medium">265.7K</p>
                            <p class="text-[14px] text-[#8C94A3]"> students</p>
                        </div>
                    </div>
                </div>


                <div class="w-[244px] h-[333px] bg-white">
                    <img src="../assets/img/Course4.svg" alt="Course1">
                    <div class="flex justify-between items-center px-[14px] mt-[14px]">
                        <p class="w-[72px] h-[20px] bg-[#EBEBFF] text-[#342F98] text-[10px] text-center font-medium">
                            MARKETING</p>
                        <p class="text-[16px] text-[#FF6636] font-semibold">$57</p>
                    </div>
                    <p class="text-[14px] learning-[20px] mt-[10px] ml-[14px] font-medium">The Complete Digital
                        Marketing<br />
                        Course - 12 Courses in 1</p>
                    <div class="flex justify-between items-center  px-[14px] pt-[29px]">
                        <div class="w-[41px] h-[20px] flex justify-between items-center">
                            <img src="../assets/img/Star.svg" alt="Star">
                            <p class="text-[14px] text-[#4E5566] font-medium">5.0</p>
                        </div>
                        <div class="flex">
                            <p class="text-[14px] text-[#4E5566] font-medium">265.7K</p>
                            <p class="text-[14px] text-[#8C94A3]"> students</p>
                        </div>
                    </div>
                </div>


                <div class="w-[244px] h-[333px] bg-white">
                    <img src="../assets/img/Course5.svg" alt="Course1">
                    <div class="flex justify-between items-center px-[14px] mt-[14px]">
                        <p class="w-[89px] h-[20px] bg-[#FFF0F0] text-[#882929] text-[10px] text-center font-medium">IT
                            & SOFTWARE</p>
                        <p class="text-[16px] text-[#FF6636] font-semibold">$57</p>
                    </div>
                    <p class="text-[14px] learning-[20px] mt-[10px] ml-[14px] font-medium">Reiki Level I, II and<br />
                        Master/Teacher Program</p>
                    <div class="flex justify-between items-center  px-[14px] pt-[29px]">
                        <div class="w-[41px] h-[20px] flex justify-between items-center">
                            <img src="../assets/img/Star.svg" alt="Star">
                            <p class="text-[14px] text-[#4E5566] font-medium">5.0</p>
                        </div>
                        <div class="flex">
                            <p class="text-[14px] text-[#4E5566] font-medium">265.7K</p>
                            <p class="text-[14px] text-[#8C94A3]"> students</p>
                        </div>
                    </div>
                </div>

            </div> -->


            <!-- 
            <div class="flex gap-[25px] mt-[25px]">

                <div class="w-[244px] h-[333px] bg-white">
                    <img src="../assets/img/Course6.svg" alt="Course1">
                    <div class="flex justify-between items-center px-[14px] mt-[14px]">
                        <p class="w-[45px] h-[20px] bg-[#FFF2E5] text-[#65390C] text-[10px] text-center font-medium">
                            MUSIC</p>
                        <p class="text-[16px] text-[#FF6636] font-semibold">$57</p>
                    </div>
                    <p class="text-[14px] learning-[20px] mt-[10px] ml-[14px] font-medium">The Complete Foundation
                        Stock<br />
                        Trading Course</p>
                    <div class="flex justify-between items-center  px-[14px] pt-[29px]">
                        <div class="w-[41px] h-[20px] flex justify-between items-center">
                            <img src="../assets/img/Star.svg" alt="Star">
                            <p class="text-[14px] text-[#4E5566] font-medium">5.0</p>
                        </div>
                        <div class="flex">
                            <p class="text-[14px] text-[#4E5566] font-medium">265.7K</p>
                            <p class="text-[14px] text-[#8C94A3]"> students</p>
                        </div>
                    </div>
                </div>


                <div class="w-[244px] h-[333px] bg-white">
                    <img src="../assets/img/Course7.svg" alt="Course1">
                    <div class="flex justify-between items-center px-[14px] mt-[14px]">
                        <p class="w-[72px] h-[20px] bg-[#EBEBFF] text-[#342F98] text-[10px] text-center font-medium">
                            MARKETING</p>
                        <p class="text-[16px] text-[#FF6636] font-semibold">$57</p>
                    </div>
                    <p class="text-[14px] learning-[20px] mt-[10px] ml-[14px] font-medium">Beginner to Pro in
                        Excel:<br />
                        Financial Modeling and Valuati...</p>
                    <div class="flex justify-between items-center  px-[14px] pt-[29px]">
                        <div class="w-[41px] h-[20px] flex justify-between items-center">
                            <img src="../assets/img/Star.svg" alt="Star">
                            <p class="text-[14px] text-[#4E5566] font-medium">5.0</p>
                        </div>
                        <div class="flex">
                            <p class="text-[14px] text-[#4E5566] font-medium">265.7K</p>
                            <p class="text-[14px] text-[#8C94A3]"> students</p>
                        </div>
                    </div>
                </div>


                <div class="w-[244px] h-[333px] bg-white">
                    <img src="../assets/img/Course8.svg" alt="Course1">
                    <div class="flex justify-between items-center px-[14px] mt-[14px]">
                        <p class="w-[105px] h-[20px] bg-[#E1F7E3] text-[#15711F] text-[10px] text-center font-medium">
                            HEALTH & FITNESS</p>
                        <p class="text-[16px] text-[#FF6636] font-semibold">$57</p>
                    </div>
                    <p class="text-[14px] learning-[20px] mt-[10px] ml-[14px] font-medium">The Python Mega Course:
                        Build<br />
                        10 Real World Applications</p>
                    <div class="flex justify-between items-center  px-[14px] pt-[29px]">
                        <div class="w-[41px] h-[20px] flex justify-between items-center">
                            <img src="../assets/img/Star.svg" alt="Star">
                            <p class="text-[14px] text-[#4E5566] font-medium">5.0</p>
                        </div>
                        <div class="flex">
                            <p class="text-[14px] text-[#4E5566] font-medium">265.7K</p>
                            <p class="text-[14px] text-[#8C94A3]"> students</p>
                        </div>
                    </div>
                </div>


                <div class="w-[244px] h-[333px] bg-white">
                    <img src="../assets/img/Course9.svg" alt="Course1">
                    <div class="flex justify-between items-center px-[14px] mt-[14px]">
                        <p class="w-[50px] h-[20px] bg-[#FFEEE8] text-[#993D20] text-[10px] text-center font-medium">
                            DESING</p>
                        <p class="text-[16px] text-[#FF6636] font-semibold">$57</p>
                    </div>
                    <p class="text-[14px] learning-[20px] mt-[10px] ml-[14px] font-medium">Copywriting - Become a<br />
                        Freelance Copywriter, your ow...</p>
                    <div class="flex justify-between items-center  px-[14px] pt-[29px]">
                        <div class="w-[41px] h-[20px] flex justify-between items-center">
                            <img src="../assets/img/Star.svg" alt="Star">
                            <p class="text-[14px] text-[#4E5566] font-medium">5.0</p>
                        </div>
                        <div class="flex">
                            <p class="text-[14px] text-[#4E5566] font-medium">265.7K</p>
                            <p class="text-[14px] text-[#8C94A3]"> students</p>
                        </div>
                    </div>
                </div>


                <div class="w-[244px] h-[333px] bg-white mb-[320px]">
                    <img src="../assets/img/Course10.svg" alt="Course1">
                    <div class="flex justify-between items-center px-[14px] mt-[14px]">
                        <p class="w-[50px] h-[20px] bg-[#FFF2E5] text-[#65390C] text-[10px] text-center font-medium">
                            LIFESTYLE</p>
                        <p class="text-[16px] text-[#FF6636] font-semibold">$57</p>
                    </div>
                    <p class="text-[14px] learning-[20px] mt-[10px] ml-[14px] font-medium">Google Analytics
                        Certification
                        -<br />Learn How To Pass The Exam</p>
                    <div class="flex justify-between items-center  px-[14px] pt-[29px]">
                        <div class="w-[41px] h-[20px] flex justify-between items-center">
                            <img src="../assets/img/Star.svg" alt="Star">
                            <p class="text-[14px] text-[#4E5566] font-medium">5.0</p>
                        </div>
                        <div class="flex">
                            <p class="text-[14px] text-[#4E5566] font-medium">265.7K</p>
                            <p class="text-[14px] text-[#8C94A3]"> students</p>
                        </div>
                    </div>
                </div>

            </div> -->
