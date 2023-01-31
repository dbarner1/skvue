<script lang="ts">
import { RouterLink } from "vue-router";

export default {
  data() {
    return {
      message: 'This is the subheader!',
      headerLinks: [
        { id: 1, title: 'Home', url: '/' },
        { id: 2, title: 'Browse', url: '/browse' },
        { id: 3, title: 'Your Cart', url: '/cart' },
        { id: 4, title: 'Specials', url: '/specials' }
      ]
    }
  }
}


</script>

<template>
  <div id="wrapper">
    <h1 id="headline">Headline</h1>
    <nav>
      <ol id="navBarWrapper">
        <li id="li" v-for="link in headerLinks">
          <RouterLink :to="{path: `${link.url}`}">
            <p id="linkText">{{link.title}}</p>
          </RouterLink>
        </li>
      </ol>
    </nav>
  </div>
</template>

<style scoped>
 #wrapper {
  padding: 10px;
  background-color: purple
 } 

 #headline {
  color: white
 }

 #navBarWrapper {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  width: 300px;
  list-style:none;
 }

 #li {
  border: 1px solid white;
 }

 #linkText {
  color: white;
  padding: 0px;
  margin: 0px;
 }
</style>