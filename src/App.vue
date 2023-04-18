<script>
  import Header from './components/Header.vue'
  import Hero from './components/Hero.vue'
  import Projects from './components/Projects.vue'
  import AboutMe from './components/AboutMe.vue'
  import Skills from './components/Skills.vue'
  import InTouch from './components/InTouch.vue'
  import Footer from './components/Footer.vue'

  export default {
    components: { Header,
      Hero,
      Projects,
      AboutMe,
      Skills,
      InTouch,
      Footer
    }
  }
</script>

<template>
  <main class="max-w-7xl m-auto">
    <Header />
    <Hero />
    <Projects />
    <AboutMe />
    <Skills />
    <InTouch />
    <Footer />
  </main>
</template>
