<template>
  <div class="container">
    <div class="row">
        <div class="col">
            <img class="img-fluid" src="https://awhendr261101.github.io/allImages/images/Daniel.png" alt="Daniel" loading="lazy">
        </div>
        <div class="col">

        </div>
    </div>
  </div>
</template>

<script setup>
import {computed, onMounted} from 'vue'
const jobTitle = computed(()=> this.$store.state.jobtitle)

onMounted(() => {
  this.$store.dispatch('getPortfolioData')
})
</script>

</script>

<style>

</style>