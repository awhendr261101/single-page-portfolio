<template>
  <div class="container">
    <h1> {{ jobTitle }} Hey there </h1>
  </div>
</template>

<script>
export default {
    name : "AboutComp",
    computed : {
        jobtitle() {
            console.log(this.$store.state);
            return this.$store.state.jobtitle
        }
    }
}
</script>

<style>

</style>