<template>
  <div class="container">
    <section class="row" id="landing">
      <Landing />
    </section>
    <section class="row" id="about"></section>
    <section class="row" id="resume"></section>
    <section class="row" id="project"></section>
    <section class="row" id="testimonials"></section>
    <section class="row" id="reachme"></section>
  </div>
</template>

<script>
// @ is an alias to /src
import Landing from '@/components/Landing.vue'
export default {

  name: 'HomeView',
  components: {
    Landing
  }
}
</script>
