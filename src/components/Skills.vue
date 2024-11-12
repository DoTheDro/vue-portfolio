<script>
    import html from '../assets/images/icon-html.png'
    import css from '../assets/images/icon-css.png'
    import javascript from '../assets/images/icon-javascript.png'
    import bootstrap from '../assets/images/icon-bootstrap.png'
    import tailwind from '../assets/images/icon-tailwind.png'
    import wordpress from '../assets/images/icon-wordpress.png'
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
                    { image: vue, title: 'Vue' },
                    { image: figma, title: 'Figma' },
                    { image: github, title: 'GitHub' },
                    { image: wordpress, title: 'WordPress' },
                    { image: php, title: 'PHP' },
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
    <div class="w-full max-w-3xl p-4 m-auto mb-36">
        <h2 data-aos="fade-left"
            data-aos-duration="800"
            data-aos-once="true"
        class="pb-5 text-3xl font-semibold text-center text-gray-100">{{ sectionHeader }}</h2>
        <div data-aos="fade-left"
            data-aos-duration="1000"
            data-aos-once="true"
        class="flex flex-col w-11/12 gap-2 p-5 m-auto custom-bg rounded-xl custom-shadow">
            <p class="text-base text-gray-100">Technologies I used and comfortable with:</p>
            <div class="flex flex-row flex-wrap gap-3 mb-5">
                <div class="flex flex-col gap-2 duration-500 lg:hover:scale-110" v-for="presentSkill in presentSkills">
                    <img :src="presentSkill['image']" :alt="presentSkill['title']" class="w-12 h-12 m-auto">
                    <p class="text-sm font-normal text-center text-gray-100">{{ presentSkill['title'] }}</p>
                </div>
            </div>
            <p class="text-base text-gray-100">Technologies I want to learn/deepen in the future:</p>
            <div class="flex flex-row flex-wrap gap-3 mb-5">
                <div class="flex flex-col gap-2 duration-500 lg:hover:scale-110" v-for="futureSkill in futureSkills">
                    <img :src="futureSkill['image']" :alt="futureSkill['title']" class="w-12 h-12 m-auto">
                    <p class="text-sm font-normal text-center text-gray-100">{{ futureSkill['title'] }}</p>
                </div>
            </div>
        </div>
    </div>
</template>