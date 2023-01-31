<script lang="ts">
import { RouterView } from 'vue-router'

export default {
  data() {
    return {
      message: 'This is the subheader!',
      headerLinks: [
        { id: 1, title: 'Browse', url: '/browse' },
        { id: 1, title: 'Your Cart', url: '/cart' },
        { id: 1, title: 'Specials', url: '/specials' }
      ]
    }
  }
}
</script>

<template>
  <div id="wrapper">
    <p>{{ message }}</p>
    <ol>
      <li v-for="link in headerLinks">
        <RouterLink to="/browse">{{ link.title }}</RouterLink>
      </li>
    </ol>
  </div>

  
</template>

<style scoped>
  #wrapper {
    background-color: magenta
  }
</style>


