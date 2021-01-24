<template>
  <div id="rectangle">
    <img src="../images/quora_logo.png" alt="" id="quora_logo">
    <input type="text" id="search_bar" placeholder="   Search Quora">
    <img src="../images/search_icon.png" alt="" id="search_icon">
    <img src="../images/home_icon.png" alt="" id="home_icon">
    <img src="../images/notification.png" alt="" id="notification">
    <h3 id="user_name">Mohit Gupta</h3>
    <img src="../images/profile-user.png" alt="" id="user_icon">

  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
#quora_logo{
  position: fixed;
  width: 125px;
  height: 79px;
  left: 26px;
  top: 0px;
}

#rectangle{
  position: fixed;
  width: 100%;
  height: 80px;
  left: 0px;
  top: 0px;
  background: #be1e1e;
  border-radius: 10px;
  margin-bottom: 100px;
}

#search_bar{
  position: fixed;
  width: 678px;
  height: 34px;
  left: 240px;
  top: 20px;
  background: #FEFEFE;
  border: 0px;
  border-radius: 10px;
}

#search_icon{
  position: fixed;
  width: 36px;
  height: 38px;
  left: 879px;
  top: 18px;
}

#home_icon{
  position: fixed;
  width: 48px;
  height: 49px;
  left: 1050px;
  top: 15px;
}

#notification{
  position: fixed;
  width: 43px;
  height: 40px;
  left: 1110px;
  top: 20px;
}

#user_name{
  position: fixed;
width: 136px;
height: 30px;
left: 1220px;
top: 3px;

font-family: Roboto;
font-style: normal;
font-weight: normal;
font-size: 24px;
line-height: 28px;

color: #000000;

}

#user_icon{
  position: absolute;
  width: 44px;
  height: 40px;
  left: 1361px;
  top: 20px;
}
</style>
