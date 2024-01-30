<script setup>
  import '@/assets/article.less'
  import SearchBar from "@/components/SearchBar.vue";
  import Posts from "@/components/Posts.vue";
  import Line from "@/components/Line.vue";
  import Footer from "@/components/footer.vue";
</script>

<template>
  <div class="article">
    <SearchBar />
    <Posts />
    <Line />
    <Footer />
  </div>
</template>

<style scoped>

</style>