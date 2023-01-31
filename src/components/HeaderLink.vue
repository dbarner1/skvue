<script setup lang="ts">
defineProps<{
  link: any
}>()
</script>

<template>
  <div id="wrapper">
    <p>Header link</p>
    
    <!-- <p id="linkText">{{ link.title }}</p> -->
  </div>
</template>

<style scoped>
  #wrapper {
    background-color: magenta
  }

  #linkText {
    color: white 
  }
</style>