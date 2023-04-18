<script>
    export default {
        data() {
            return {
                sectionHeader: 'Get in Touch'
            }
        }
    }
</script>

<template>
    <div class="w-full p-4 mb-36 flex flex-col gap-4">
        <h2 data-aos="zoom-in"
            data-aos-duration="700"
            data-aos-once="true"
        class="text-gray-100 text-3xl font-semibold text-center pb-5">{{ sectionHeader }}</h2>
        <div data-aos="zoom-in"
            data-aos-duration="900"
            data-aos-once="true"
        class="w-full flex flex-col">
            <h5 class="text-gray-100 text-center text-lg">LinkedIn:</h5>
            <a href="https://www.linkedin.com/in/dothedro/" class="text-gray-100 text-center text-lg" target="_blank">Andrew Buhat</a>
        </div>
        <div data-aos="zoom-in"
            data-aos-duration="1100"
            data-aos-once="true"
        class="w-full flex flex-col">
            <h5 class="text-gray-100 text-center text-lg">Email:</h5>
            <a href="mailto:drewcarlo132@gmail.com" class="text-gray-100 text-center text-lg" target="_blank">drewcarlo132@gmail.com</a>
        </div>
    </div>
</template>