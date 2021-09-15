<template>
  <div>
      <navbar/>
      <Demo />
      <footer/>
  </div>
</template>

<script>
import Demo from '../components/Demo.vue'
import navbar from '../components/navbar.vue'
import footer from '../components/footer.vue'
export default {
    components: {
        Demo,
        navbar,
        footer
    }
}
</script>

<style>

</style>