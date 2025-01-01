<template>
  <Home :profile="profile"/>

</template>

<script>
import profile from './info/profile.json'
import Home from './components/views/Home.vue'

export default {
  name: 'App',
  components: {
    Home
  },
  data(){
    return {
      profile:profile
    }
  }
}
</script>

<style>

</style>
