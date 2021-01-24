<template>
  <div id="landing_page">
    <Category></Category>
    <div>
    <AskAQuestion></AskAQuestion>
    <button id="ask_question">Ask Question</button>
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
import AskAQuestion from '../components/AskAQuestion.vue'
import Category from '../components/Category.vue'
import Post from '../components/Post.vue'
export default {
  components: { Post, Category, Advertisement, AskAQuestion },
  name: 'Homepage'
}

</script>

<style scoped>
#landing_page{
  display: flex;
}
#ask_question{
  margin-left: 870px;
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 10px;
  padding-top: 10px;
  border-radius: 10px;
  background: #b82929;
  color: white;
  margin-bottom: 10px;

}
</style>
