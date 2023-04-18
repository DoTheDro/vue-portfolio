<script>
    export default {
        data() {
            return {
                contents: [
                    { title: 'GitHub', link: 'https://github.com/DoTheDro' },
                    { title: 'LinkedIn', link: 'https://www.linkedin.com/in/dothedro/' },
                ]
            }
        }
    }
</script>

<template>
    <div data-aos="fade-up"
        data-aos-duration="500"
        data-aos-once="true"
    class="p-4 gap-6 flex justify-center">
        <a class="text-gray-100 text-lg" v-for="content in contents" :href="content['link']" target="_blank">{{ content['title'] }}</a>
    </div>
</template>