<template>
<div>
<div id="my_profile">
<Category></Category>
<div>
  <img src="../images/profile-user.png" alt="" id="profile_pic">
</div>
<div>
    <h1 id="profile_name">{{ profileDetails.businessName }}</h1>
    <h4 id="profile_rating">Profile Rating: 2900</h4>
    <div style="display: flex;">
      <p style="margin-left: 35px">10 Followers</p>
      <p style="margin-left: 10px">10 Following</p>
      <button id="follow_button">Follow</button>
    </div>
    <p id="email_id">Email ID: {{ profileDetails.businessEmail }}</p>
    <div>
    <p id="bio">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Nesciunt adipisci possimus nobis distinctio consectetur. Earum, laudantium saepe fuga magnam laborum ea neque repudiandae id rerum nam, ducimus cupiditate facere consectetur.</p>
    </div>
</div>
<Advertisement></Advertisement>
</div>
<Post :businessName="profileDetails.businessName"></Post>
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
import axios from 'axios'
export default {
  components: { Category, Advertisement, Post },
  data: () => {
    return {
      profileDetails: {}
    }
  },
  mounted () {
    axios.get('http://10.177.1.217:9007/profile/getBusinessProfileDetails/abc')
      .then(response => {
        console.log(response)
        console.log()
        this.profileDetails = response.data.data
      })
  }
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
#email_id{
  margin-right: 220px;
}
#profile_name{
  margin-right: 220px;
  margin-top: 30px;
}
#profile_rating{
  margin-right: 250px;
  margin-top: 20px;
}
#follow_button{
  margin-top: 10px;
  margin-left: 150px;
  padding-left: 20px;
  padding-right: 20px;
  padding-bottom: 10px;
  padding-top: 10px;
  border-radius: 10px;
  background: #b82929;
  color: white;
  margin-bottom: 10px;
}
#bio{
  position: relative;
  right: 150px;
  text-align: left;
  top: 10px;
}
</style>
