<template>
  <div class="container">
    <Card>
        
    </Card>
  </div>
</template>

<script>
import Card from '@/components/Card.vue'
export default {
    name : "AboutComp",
    components : {
        Card
    },
    computed : {
        jobtitle() {
            console.log(this.$store.state.jobtitle, "About");
            return this.$store.state.education
        },
        about(){
            console.log(this.$store.state, "About");
            return this.$store.state.about
        }
    }
}
</script>

<style>

</style>