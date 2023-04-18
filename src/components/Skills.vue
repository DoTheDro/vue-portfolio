<script>
    import html from '../assets/images/icon-html.png'
    import css from '../assets/images/icon-css.png'
    import javascript from '../assets/images/icon-javascript.png'
    import bootstrap from '../assets/images/icon-bootstrap.png'
    import tailwind from '../assets/images/icon-tailwind.png'
    import react from '../assets/images/icon-react.png'
    import vue from '../assets/images/icon-vue.png'
    import figma from '../assets/images/icon-figma.png'
    import github from '../assets/images/icon-github.png'
    import node from '../assets/images/icon-node.png'
    import php from '../assets/images/icon-php.png'

    export default {
        data() {
            return {
                sectionHeader: 'My Skills',
                presentSkills: [
                    { image: html, title: 'HTML' },
                    { image: css, title: 'CSS' },
                    { image: javascript, title: 'JavaScript' },
                    { image: bootstrap, title: 'Bootstrap' },
                    { image: tailwind, title: 'Tailwind' },
                    { image: react, title: 'React' },
                    { image: vue, title: 'Vue' },
                    { image: figma, title: 'Figma' },
                    { image: github, title: 'GitHub' },
                ],
                futureSkills: [
                    { image: vue, title: 'Vue' },
                    { image: node, title: 'Node' },
                    { image: php, title: 'PHP' },
                ]
            }
        }
    }
</script>

<template>
    <div class="w-full p-4 mb-36 max-w-3xl m-auto">
        <h2 data-aos="fade-left"
            data-aos-duration="800"
            data-aos-once="true"
        class="text-gray-100 text-3xl font-semibold text-center pb-5">{{ sectionHeader }}</h2>
        <div data-aos="fade-left"
            data-aos-duration="1000"
            data-aos-once="true"
        class="custom-bg w-11/12 rounded-xl m-auto p-5 custom-shadow flex flex-col gap-2">
            <p class="text-gray-100 text-base">Technologies I am knowledgeable with:</p>
            <div class="flex flex-row flex-wrap gap-3 mb-5">
                <div class="flex flex-col gap-2 duration-500 lg:hover:scale-110" v-for="presentSkill in presentSkills">
                    <img :src="presentSkill['image']" :alt="presentSkill['title']" class="w-12 h-12 m-auto">
                    <p class="text-gray-100 text-center text-sm font-normal">{{ presentSkill['title'] }}</p>
                </div>
            </div>
            <p class="text-gray-100 text-base">Technologies I want to learn/deepen in the future:</p>
            <div class="flex flex-row flex-wrap gap-3 mb-5">
                <div class="flex flex-col gap-2 duration-500 lg:hover:scale-110" v-for="futureSkill in futureSkills">
                    <img :src="futureSkill['image']" :alt="futureSkill['title']" class="w-12 h-12 m-auto">
                    <p class="text-gray-100 text-center text-sm font-normal">{{ futureSkill['title'] }}</p>
                </div>
            </div>
        </div>
    </div>
</template>