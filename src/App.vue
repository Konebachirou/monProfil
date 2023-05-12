<script setup>
import Header from './components/Header.vue'
import Home from './components/Home.vue'
import About from './components/About.vue'
import Skills from './components/Skills.vue';
import Contacts from './components/Contacts.vue';
import Education from './components/education/Education.vue';
import Experienece from './components/experience/Experience.vue'
import Backtop from './components/BackTop.vue'
</script>

<template>
<Header />
<Home/>
  <main id="main">
    <About />
    <Education />
    <Experienece/>
    <Skills />
    <Contacts/>
  </main>
  <Backtop/>
</template>

<!-- <style scoped>

</style> -->
