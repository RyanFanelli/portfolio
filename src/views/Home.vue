<template>
  <div class="home">
    <CyanCat />
    <Desktop />
    <NavBar />
  </div>
</template>

<script>
// @ is an alias to /src
import Desktop from '@/components/Desktop.vue'
import NavBar from '@/components/NavBar.vue'
import CyanCat from '@/components/CyanCat.vue'


export default {
  name: 'Home',
  components: {
    CyanCat,
    Desktop,
    NavBar
  },
  mounted() {
    console.warn('this message will self destruct in 30s')
    setTimeout(() => {
      console.error('ka-boom!')
    }, 1000 *30)
  },
}
</script>

<style>
  body {
  margin: 0;
  background-color: rgb(3,128,131)
}
</style>
