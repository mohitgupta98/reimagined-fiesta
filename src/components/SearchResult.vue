<template>
<div id="rectangle">
  <div id="user_details">
    <img src="../images/profile-user.png" alt="" id="user_icon">
    <div>
      <h4 id="user">Mohit Gupta</h4>
      <p id="user_rating">   User Rating : 2900 </p>
    </div>
  </div>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
#rectangle{
  width: 663px;
  height: 120px;
  background: rgb(235, 232, 232);
  margin-left: 360px;
  margin-bottom: 20px;
  border-radius: 10px;
}
#user_icon{
  width: 104px;
  height: 100px;
  margin-top: 10px;
  margin-left: 30px;
}
#user{
  width: 150px;
  margin-top: 20px;
  /* margin-left: 5px;
  margin-right: 460px; */
}
#user_details{
  display: flex;
}
#user_rating{
  margin-left: 25px;
}
</style>
