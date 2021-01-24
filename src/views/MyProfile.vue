<template>
<div>
<div id="my_profile">
<Category></Category>
<div>
  <img src="../images/profile-user.png" alt="" id="profile_pic">
</div>
<div>
    <h1 id="profile_name">Mohit Gupta</h1>
    <h4 id="profile_rating">Profile Rating: 2900</h4>
    <div style="display: flex;">
      <p style="margin-left: 33px">Followers</p>
      <p style="margin-left: 25px">Following</p>
      <img src="../images/edit.png" alt="" id="edit_icon">
    </div>
    <div>
    <p id="bio">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nesciunt adipisci possimus nobis distinctio consectetur. Earum, laudantium saepe fuga magnam laborum ea neque repudiandae id rerum nam, ducimus cupiditate facere consectetur.</p>
    </div>
</div>
<Advertisement></Advertisement>
</div>
<Post></Post>
<Post></Post>
<Post></Post>
<Post></Post>
<Post></Post>
</div>
</template>

<script>
import Advertisement from '../components/Advertisement.vue'
import Category from '../components/Category.vue'
import Post from '../components/Post.vue'
export default {
  components: { Category, Advertisement, Post }

}
</script>

<style scoped>
#my_profile{
  display: flex;
  width: 663px;
  height: auto;
  background: rgb(235, 232, 232);
  margin-left: 360px;
  margin-bottom: 20px;
  border-radius: 10px;
}
#profile_pic{
  width: 170px;
  height: 170px;
  margin-left: 20px;
  margin-top: 20px;
  margin-bottom: 20px;
}
#profile_name{
  position: relative;
  right: 110px;
  /* margin-left: 30px;
  margin-top: 30px; */
}
#profile_rating{
  position: relative;
  right: 130px;
  /* margin-left: 30px;
  margin-top: 30px; */
}
#edit_icon{
  position: relative;
  left: 230px;
  top: 17px;
  width: 20px;
  height: 20px;
}
#bio{
  position: relative;
  right: 150px;
  text-align: left;
  top: 10px;
}
</style>
