<template>
  <div class="template">
    <div class="text-center">
      <h4>상세페이지</h4>
      <h5>{{ blogData[$route.params.id].title }}</h5>
      <p>{{ blogData[$route.params.id].title }}</p>
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DetailView',
  props: {
    blogData: Array,
  },
};
</script>

<style></style>
