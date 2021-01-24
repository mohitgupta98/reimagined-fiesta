<template>
  <div id="landing_page">
    <Category></Category>
    <div>
    <Post></Post>
    <Post></Post>
    <Post></Post>
    <Post></Post>
    </div>
    <div>
      <Advertisement></Advertisement>
      <Advertisement></Advertisement>
    </div>
  </div>
</template>

<script>
import Advertisement from '../components/Advertisement.vue'
import Category from '../components/Category.vue'
import Post from '../components/Post.vue'
export default {
  components: { Post, Category, Advertisement },
  name: 'Homepage'
}
</script>

<style>
#landing_page{
  display: flex;
}
</style>
