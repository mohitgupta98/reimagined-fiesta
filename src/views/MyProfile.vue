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
      <p style="margin-left: 33px">{{ followersCount }}Followers</p>
      <p style="margin-left: 25px">{{ followingCount }}Following</p>
      <img src="../images/edit.png" alt="" id="edit_icon">
    </div>
    <div>
    <p id="bio">{{profileDetails.businessDescription}}</p>
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
import axios from 'axios'
export default {
  components: { Category, Advertisement, Post },
  data: () => {
    return {
      profileDetails: {},
      followersCount: 0,
      followingCount: 0
    }
  },
  mounted () {
    axios.get('http://10.177.1.217:9007/profile/getUserProfileDetails/1234')
      .then(response => {
        console.log(response)
        console.log()
        this.profileDetails = response.data.data
      })
    axios.get('http://10.177.1.217:9007/profile/getFollowersCount/Dali')
      .then(response => {
        console.log(response)
        console.log()
        this.followersCount = response.data
      })
    axios.get('http://10.177.1.217:9007/profile/getFollowingCount/3')
      .then(response => {
        console.log(response)
        console.log()
        this.followingCount = response.data
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
#profile_name{
  margin-right: 220px;
  margin-top: 30px;
}
#profile_rating{
  margin-right: 250px;
  margin-top: 20px;
}
#edit_icon{
  width: 20px;
  height: 20px;
  margin-top: 20px;
  margin-left: 230px;
}
#bio{
  position: relative;
  right: 150px;
  text-align: left;
  top: 10px;
}
</style>
