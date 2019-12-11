<template>
  <div>
    <Navbar />
    <nuxt />
  </div>
</template>

<script>
import Navbar from '@/components/Navbar'
import axios from 'axios'

axios.defaults.headers.common['user-key'] = 'user_key'
axios.defaults.headers.common['X-Requested-With'] = 'XMLHttpRequest'

export default {
  components: {
    Navbar
  }
}
</script>

<style>
</style>
