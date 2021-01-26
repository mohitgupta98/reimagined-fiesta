<template>
  <div id="comments_page">
    <div>
      <Category></Category>
    </div>
    <div>
      <h2 style="margin-right: 18%">Comments</h2>
      <textarea id="ask_a_question" placeholder="Write your Comment" rows="3" cols="45"></textarea>
      <Comments></Comments>
      <Comments></Comments>
      <Comments></Comments>
      <Comments></Comments>
      <Comments></Comments>
    </div>
    <div>
      <Advertisement></Advertisement>
    </div>
  </div>
</template>

<script>
import Advertisement from '../components/Advertisement.vue'
import Category from '../components/Category.vue'
import Comments from '../components/Comments.vue'
export default {
  components: { Category, Comments, Advertisement }

}
</script>

<style scoped>
#comments_page{
  display: flex;
}
textarea{
  margin-left: 355px;
  border-radius: 10px;
  font-size: 24px;
  margin-bottom: 5px;
}
</style>
