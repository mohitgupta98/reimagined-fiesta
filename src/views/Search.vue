<template>
<div class="newclass">
  <Category></Category>
  <div>
    <h2>Search Results for Mohit Gupta</h2>
    <SearchResult></SearchResult>
    <SearchResult></SearchResult>
    <SearchResult></SearchResult>
    <SearchResult></SearchResult>
    <SearchResult></SearchResult>
  </div>
  <div>
    <Advertisement></Advertisement>
  </div>
</div>
</template>

<script>
import Advertisement from '../components/Advertisement.vue'
import Category from '../components/Category.vue'
import SearchResult from '../components/SearchResult.vue'
export default {
  components: { SearchResult, Category, Advertisement },
  name: 'Search'
}
</script>

<style scoped>
.newclass{
  margin-top: 100px;
  display: flex;
}
h2{
  margin-left: 120px;
}
</style>
