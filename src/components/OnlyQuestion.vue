<template>
  <div id="rectangle">
    <h2>This is supposed to be a question?</h2>
    <img src="../images/like.png" alt="" id="like_icon">
    <img src="../images/dislike.png" alt="" id="dislike_icon">
    <img src="../images/comment.png" alt="" id="comment_icon">
    <router-link to="/answerthisquestion">
    <button id="answer_button">Answer this</button>
    </router-link>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
#answer_button{
  margin-left: 20px;
  margin-bottom: 10px;
}
#rectangle{
  width: 663px;
  height: auto;
  background: rgb(235, 232, 232);
  margin-left: 360px;
  margin-bottom: 20px;
  border-radius: 10px;
}
.responder_info{
  display: flex;
  margin-bottom: 20px;
}
#user_icon{
  width: 44px;
  height: 40px;
  margin-top: 10px;
  margin-left: 10px;
}
#answer_responder{
  width: 100px;
  margin-top: 10px;
  margin-left: 10px;
  margin-right: 350px;
  word-break: break-all;
  white-space: nowrap;
}
h2{
  width: 663px;
  text-align: left;
  padding-left: 20px;
  padding-right: 20px;
  margin-top: 0px;
}
#date{
  width: auto;
  margin-top: 10px;
  margin-left: 0px;
  margin-right: 570px;
  word-break: break-all;
  white-space: nowrap;
}
#answer{
  text-align: left;
  padding-bottom: 5px;
  padding-left: 20px;
  padding-right: 20px;
}
#like_icon{
  position: relative;
  right: 250px;
  width: 44px;
  height: 40px;
  margin-top: 10px;
  margin-left: 90px;
}
#dislike_icon{
  position: relative;
  right: 220px;
  width: 40px;
  height: 30px;
  margin-top: 10px;
  margin-left: 0px;
}
#comment_icon{
  position: relative;
  right: 190px;
  width: 40px;
  height: 30px;
  margin-top: 10px;
  margin-left: 0px;
}
</style>
