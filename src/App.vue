<template>
  <div class="wrapper" >
    <NavBar />

    <main class="container-fluid">
      <router-view/>
      <About />
    </main>

    <Footer />
  
  </div>
</template>

<script>
import NavBar from '@/components/NavBar.vue'
import Footer from '@/components/Footer.vue'
import About from '@/components/About.vue'

export default {
  components: {
    NavBar, Footer, About,
  }, 
  computed : {
    jobTitle(){
      return this.$store.state.jobTitle
    }, 
    about(){ return this.$store.state.about},
    education(){ return this.$store.state.education},
    experience(){ return this.$store.state.experience},
    skills(){ return this.$store.state.skills},
    testimonials(){ return this.$store.state.testimonials},
    projects(){ return this.$store.state.projects},
  },
  mounted(){ 
    console.log("here");
    return this.$store.dispatch('getPortfolioData')
  }
}
</script>

<style src="./assets/css/style.css">

</style>
