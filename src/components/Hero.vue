<script>
    export default {
        data() {
            return {
                name: 'Andrew Buhat',
                job: 'Web Developer',
                briefing: 'I am a web developer who loves to learn and create new things.'
            }
        }
    }
</script>

<template>
    <div data-aos="fade-up" 
        data-aos-duration="700"
        data-aos-once="true"
    class="w-full p-4 flex flex-col justify-center gap-2 h-screen-93">
        <h1 class="text-gray-100 text-5xl font-semibold">{{ name }}.</h1>
        <h4 class="text-gray-100 text-2xl font-medium">{{ job }}</h4>
        <h5 class="text-gray-100 text-base font-normal">{{ briefing }}</h5>
        <div class="flex pt-8">
            <a href="mailto:drewcarlo132@gmail.com" class="text-gray-100 text-base p-3 bg-blue-800 rounded-md cursor-pointer duration-500 lg:hover:scale-110">Contact Me</a>
        </div>
    </div>
</template>