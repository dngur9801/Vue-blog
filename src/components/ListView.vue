<template>
  <div class="template">
    <div class="container mt-4" v-for="item in blogData" :key="item">
      <h5 @click="$router.push('/detail/' + item.number)">{{ item.title }}</h5>
      <p>{{ item.date }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ListView',
  props: {
    blogData: Array,
  },
};
</script>

<style></style>
