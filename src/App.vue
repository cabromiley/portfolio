<template>
  <Hero />
  <Skills />
  <Portfolio />
</template>

<script>
import Hero from "@/components/Hero.vue"
import Skills from "@/components/Skills.vue"
import Portfolio from "@/components/Portfolio.vue"
export default {
  name: 'App',
  components: { Hero, Skills, Portfolio }
}
</script>
