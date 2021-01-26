<template>
  <div id="landing_page">
    <Category></Category>
    <div>
      <h2>Unanswered Questions</h2>
      <OnlyQuestion></OnlyQuestion>
      <OnlyQuestion></OnlyQuestion>
      <OnlyQuestion></OnlyQuestion>
      <OnlyQuestion></OnlyQuestion>
      <OnlyQuestion></OnlyQuestion>

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
import OnlyQuestion from '../components/OnlyQuestion.vue'
export default {
  components: { Category, Advertisement, OnlyQuestion },
  name: 'Homepage'
}

</script>

<style scoped>
#landing_page{
  display: flex;
}
#ask_question_category{
  margin-left: 800px;
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 10px;
  padding-top: 10px;
  border-radius: 10px;
  background: #b82929;
  color: white;
  margin-bottom: 10px;

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
