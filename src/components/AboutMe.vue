<script>
    export default {
        data() {
            return {
                sectionHeader: 'About Me'
            }
        }
    }
</script>

<template>
    <div class="w-full max-w-3xl p-4 m-auto mb-36">
        <h2 data-aos="fade-right"
            data-aos-duration="800"
            data-aos-once="true"
        class="pb-5 text-3xl font-semibold text-center text-gray-100">{{ sectionHeader }}</h2>
        <div data-aos="fade-right"
            data-aos-duration="1000"
            data-aos-once="true"
        class="flex flex-col items-center w-11/12 gap-5 p-5 m-auto custom-bg rounded-xl custom-shadow">
            <p class="text-lg font-normal text-center text-gray-100">Since I was a kid I like to solve puzzles and play with blocks turns out programming is almost the same. It needs different kinds of approaches and the use of different blocks to solve a specific problem.</p>
            <p class="text-lg font-normal text-center text-gray-100">I started programming about 7 years ago mainly in Arduino but then I decided to go into web development.</p>
            <p class="text-lg font-normal text-center text-gray-100">When I learn something new, I like to write it down in my own words and how I understand it so I don't forget it.</p>
            <a class="px-5 py-3 text-gray-100 duration-500 bg-blue-700 rounded w-max lg:hover:scale-110" href="https://drive.google.com/file/d/1FDHOcqqo4kpRAbtMHx4LHl_jKjGp5Hin/view?usp=sharing" target="_blank">Download CV</a>
        </div>
    </div>
</template>