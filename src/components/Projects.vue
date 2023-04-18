<script>
    import project1 from '../assets/images/ac-store-image.png'
    import project2 from '../assets/images/art-service-image.png'
    import project3 from '../assets/images/kidscella-image.png'
    import project4 from '../assets/images/d-kicks-image.png'
    import project5 from '../assets/images/deymburger-image.png'
    import iconvue from '../assets/images/icon-vue.png'
    import icontailwind from '../assets/images/icon-tailwind.png'
    import iconreact from '../assets/images/icon-react.png'

    export default {
        data() {
            return {
                sectionName: 'Projects',
                projects: [
                    { title: 'Deymburger', 
                    image: project5, 
                    description: 'A personal project build with Vue and Tailwind. This project widened my knowledge in Vue. Also learned and added Swiper and AOS', 
                    technology: [
                        { techImage: iconvue, techName: 'Vue' },
                        { techImage: icontailwind, techName: 'Tailwind' },
                    ],
                    links: [
                        { linkTo: 'GitHub', uriLink: 'https://github.com/DoTheDro/vue-deymburger' },
                        { linkTo: 'Live Demo', uriLink: 'https://deymburger.vercel.app/' },
                    ]
                    },
                    { title: 'D Kicks Project', 
                    image: project4, 
                    description: 'A personal project build with Vue and Tailwind. Learned fundamentals of Vue, event handlers, and data management', 
                    technology: [
                        { techImage: iconvue, techName: 'Vue' },
                        { techImage: icontailwind, techName: 'Tailwind' },
                    ],
                    links: [
                        { linkTo: 'GitHub', uriLink: 'https://github.com/DoTheDro/vue-d-kicks' },
                        { linkTo: 'Live Demo', uriLink: 'https://d-kicks.vercel.app/' },
                    ]
                    },
                    { title: 'Kidscella', 
                    image: project3, 
                    description: 'A local tutorial service. With this project, I added a new technology aside from React to increase my skill', 
                    technology: [
                        { techImage: iconreact, techName: 'React' },
                        { techImage: icontailwind, techName: 'Tailwind' },
                    ],
                    links: [
                        { linkTo: 'GitHub', uriLink: 'https://github.com/DoTheDro/kidscella' },
                        { linkTo: 'Live Demo', uriLink: 'https://kidscella.vercel.app/' },
                    ]
                    },
                    { title: 'Art\'s Service', 
                    image: project2, 
                    description: 'A personal project of mine. Through this project, I learned a grasp of how React Router Works', 
                    technology: [
                        { techImage: iconreact, techName: 'React' },
                    ],
                    links: [
                        { linkTo: 'GitHub', uriLink: 'https://github.com/DoTheDro/art-service' },
                        { linkTo: 'Live Demo', uriLink: 'https://art-service.vercel.app/' },
                    ]
                    },
                    { title: 'AC-Store', 
                    image: project1, 
                    description: 'A personal project of mine. Through this project, I learned a grasp of how React Router Works', 
                    technology: [
                        { techImage: iconreact, techName: 'React' },
                    ],
                    links: [
                        { linkTo: 'GitHub', uriLink: 'https://github.com/DoTheDro/vite-react-2' },
                        { linkTo: 'Live Demo', uriLink: 'https://dothedro.github.io/vite-react-2/' },
                    ]
                    },
                ],
            }
        },
    }


</script>

<template>
    <div class="w-full p-4 mb-36 flex flex-col gap-6">
        <h2 data-aos="flip-down"
            data-aos-duration="800"
            data-aos-once="true"
        class="text-gray-100 text-3xl font-semibold text-center pb-5">{{ sectionName }}</h2>
        <div data-aos="flip-down"
            data-aos-duration="900"
            data-aos-once="true"
        class="flex flex-row flex-wrap">
            <div class="w-full sm:w-1/2 p-3 lg:w-4/12" v-for="(project, key) in projects">
                <div class="rounded-md border-2 border-white px-4 py-7 flex flex-col gap-4 min-h-standard min-h-full justify-between">
                    <div>
                        <img class="rounded h-40 m-auto duration-500 lg:hover:scale-110" :src="project['image']" :alt="project['title']">
                    </div>
                    <div class="flex flex-col gap-6">
                        <div>
                            <h3 class="text-gray-100 text-2xl font-medium">{{ project['title'] }}</h3>
                        </div>
                        <div>
                            <p class="text-gray-100 text-lg">{{ project['description'] }}</p>
                        </div>
                        <div>
                            <p class="text-gray-100 text-base mb-3">Technology Used</p>
                            <div class="flex gap-3">
                                <div v-for="value in project['technology']" class="flex flex-col items-center justify-end gap-1 duration-500 lg:hover:scale-110">
                                    <img class="w-10 h-10" :src="value['techImage']" :alt="value['techName']">
                                    <p class="text-gray-100 text-sm">{{ value['techName'] }}</p>
                                </div>
                            </div>
                        </div>
                        <div class="flex justify-center gap-8 sm:justify-start">
                            <div v-for="value in project['links']">
                                <a :href="value['uriLink']" class="flex justify-center py-2 rounded-md custom-shadow bg-gray-100 text-gray-900 text-base w-24 duration-500 sm:text-lg sm:w-28 lg:hover:scale-110" target="_blank">{{ value['linkTo'] }}</a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>