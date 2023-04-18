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
    <div class="w-full p-4 mb-36 max-w-3xl m-auto">
        <h2 data-aos="fade-right"
            data-aos-duration="800"
            data-aos-once="true"
        class="text-gray-100 text-3xl font-semibold text-center pb-5">{{ sectionHeader }}</h2>
        <div data-aos="fade-right"
            data-aos-duration="1000"
            data-aos-once="true"
        class="custom-bg rounded-xl w-11/12 m-auto p-5 flex flex-col items-center gap-5 custom-shadow">
            <p class="text-gray-100 text-lg text-center font-normal">Since I was a kid I like to solve puzzles and play with blocks turns out programming is almost the same. It needs different kinds of approaches and the use of different blocks to solve a specific problem.</p>
            <p class="text-gray-100 text-lg text-center font-normal">I started programming about 7 years ago mainly in Arduino but then I decided to go into web development.</p>
            <p class="text-gray-100 text-lg text-center font-normal">When I learn something new, I like to write it down in my own words and how I understand it so I don't forget it.</p>
            <a class="py-3 px-5 bg-blue-700 w-max rounded text-gray-100 duration-500 lg:hover:scale-110" href="https://drive.google.com/file/d/18NwabgkgIGGRSblg62FQ3AB3A24fDMNd/view" target="_blank">Download CV</a>
        </div>
    </div>
</template>