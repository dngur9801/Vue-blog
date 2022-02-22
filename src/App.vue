<template>
  <div class="template">
    <NavBar />
    <div class="container">
      <router-link to="/">홈페이지</router-link>
      <router-link to="/list">리스트페이지</router-link>
      <router-view :blogData="blogData"></router-view>
      <!-- <ListView v-for="item in blogData" :key="item" :item="item" /> -->
    </div>
  </div>
</template>

<script>
import blogData from './assets/blog.js';
import ListView from './components/ListView.vue';
import NavBar from './components/NavBar.vue';
export default {
  name: 'App',
  data() {
    return {
      blogData: blogData,
    };
  },
  components: {
    ListView: ListView,
    NavBar: NavBar,
  },
};
</script>

<style></style>
