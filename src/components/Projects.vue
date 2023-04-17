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
                projects: [
                    { id: 1, 
                    title: 'AC-Store', 
                    image: project1, 
                    description: 'A personal project of mine. Through this project, I learned a grasp of how React Router Works', 
                    technology: [
                        { techImage: iconreact, techName: 'React' },
                    ]
                    },
                    { id: 2, 
                    title: 'Art\'s Service', 
                    image: project2, 
                    description: 'A personal project of mine. Through this project, I learned a grasp of how React Router Works', 
                    technology: [
                        { techImage: iconreact, techName: 'React' },
                    ]
                    },
                    { id: 3, 
                    title: 'Kidscella', 
                    image: project3, 
                    description: 'A local tutorial service. With this project, I added a new technology aside from React to increase my skill', 
                    technology: [
                        { techImage: iconreact, techName: 'React' },
                        { techImage: icontailwind, techName: 'Tailwind' },
                    ]
                    },
                    { id: 4, 
                    title: 'D Kicks Project', 
                    image: project4, 
                    description: 'A personal project build with Vue and Tailwind. Learned fundamentals of Vue, event handlers, and data management', 
                    technology: [
                        { techImage: iconvue, techName: 'Vue' },
                        { techImage: icontailwind, techName: 'Tailwind' },
                    ]
                    },
                    { id: 5, 
                    title: 'Deymburger', 
                    image: project5, 
                    description: 'A personal project build with Vue and Tailwind. This project widened my knowledge in Vue. Also learned and added Swiper and AOS', 
                    technology: [
                        { techImage: iconvue, techName: 'Vue' },
                        { techImage: icontailwind, techName: 'Tailwind' },
                    ]
                    },
                ]
            }
        }
    }
</script>

<template>
    <div v-for="project in projects">
        <div>
            <img :src="project['image']" :alt="project['title']">
        </div>
        <div>
            <h2 class="text-gray-100 text-4xl">{{ project['title'] }}</h2>
            <p class="text-gray-100 text-xl">{{ project['description'] }}</p>
        </div>
        <div v-for="technology in project.technology">
            <div>
                <img :src="technology.techImage" :alt="techName">
                <p>{{ technology.techName }}</p>
            </div>
        </div>
    </div>
</template>