<template>
  <div id="rectangle">
    <div class="responder_info">
      <img src="../images/profile-user.png" alt="" id="user_icon">
      <span id="answer_responder">Mohit Gupta</span>
      <p id="date">10 December 2021</p>
    </div>
    <router-link to="question">
    <h2>This is supposed to be a question?</h2>
    </router-link>
    <p id="answer">Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus distinctio facilis repudiandae aspernatur accusamus quo dicta, repellendus accusantium ad nihil, animi perspiciatis ipsam, debitis nisi perferendis optio nostrum rerum provident. Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium, ullam! Earum obcaecati recusandae nemo unde explicabo iste culpa voluptates, voluptatem aliquid maiores doloremque impedit tenetur vero! Itaque iusto rem non! Lorem ipsum dolor sit amet consectetur adipisicing elit. Architecto, quae autem magnam minus ex saepe facere aliquam porro iusto totam corrupti quaerat, obcaecati accusamus natus rerum libero, inventore vero corporis!</p>
    <img :src="like" alt="" id="like_icon" @click="changeLike" class="like" >
    <img :src="dislike" alt="" id="dislike_icon" @click="changeDislike" class="dislike">
    <router-link to="/comments">
    <img src="../images/comment.png" alt="" id="comment_icon">
    </router-link>
  </div>
</template>

<script>
export default {
  data: () => {
    return {
      like: 'https://www.flaticon.com/svg/vstatic/svg/633/633759.svg?token=exp=1611566290~hmac=adb18c3aff33a26105e6a72408673378',
      dislike: 'https://www.flaticon.com/svg/vstatic/svg/2107/2107811.svg?token=exp=1611638411~hmac=080d622ab8c26491007ca74a4ebe781a'
    }
  },
  methods: {
    changeLike (event) {
      if (this.like === 'https://www.flaticon.com/svg/vstatic/svg/633/633759.svg?token=exp=1611566290~hmac=adb18c3aff33a26105e6a72408673378' && this.dislike === 'https://www.flaticon.com/svg/vstatic/svg/2107/2107811.svg?token=exp=1611638411~hmac=080d622ab8c26491007ca74a4ebe781a') {
        this.like = 'https://www.flaticon.com/svg/vstatic/svg/633/633991.svg?token=exp=1611566313~hmac=fc5c1e2ba17b84f97b723ce6b4b92d04'
      }else if(this.like === 'https://www.flaticon.com/svg/vstatic/svg/633/633759.svg?token=exp=1611566290~hmac=adb18c3aff33a26105e6a72408673378' && this.dislike === 'https://www.flaticon.com/svg/vstatic/svg/2107/2107616.svg?token=exp=1611638176~hmac=c5331029c9417f905a16d251adad1871'){
        this.like = 'https://www.flaticon.com/svg/vstatic/svg/633/633991.svg?token=exp=1611566313~hmac=fc5c1e2ba17b84f97b723ce6b4b92d04'
        this.dislike = 'https://www.flaticon.com/svg/vstatic/svg/2107/2107811.svg?token=exp=1611638411~hmac=080d622ab8c26491007ca74a4ebe781a'
      } 
      else {
        this.like = 'https://www.flaticon.com/svg/vstatic/svg/633/633759.svg?token=exp=1611566290~hmac=adb18c3aff33a26105e6a72408673378'
      }
    },
    changeDislike () {
      if (this.dislike === 'https://www.flaticon.com/svg/vstatic/svg/2107/2107811.svg?token=exp=1611638411~hmac=080d622ab8c26491007ca74a4ebe781a' && this.like === 'https://www.flaticon.com/svg/vstatic/svg/633/633759.svg?token=exp=1611566290~hmac=adb18c3aff33a26105e6a72408673378') {
        this.dislike = 'https://www.flaticon.com/svg/vstatic/svg/2107/2107616.svg?token=exp=1611638176~hmac=c5331029c9417f905a16d251adad1871'
      } else if(this.dislike === 'https://www.flaticon.com/svg/vstatic/svg/2107/2107811.svg?token=exp=1611638411~hmac=080d622ab8c26491007ca74a4ebe781a' && this.like === 'https://www.flaticon.com/svg/vstatic/svg/633/633991.svg?token=exp=1611566313~hmac=fc5c1e2ba17b84f97b723ce6b4b92d04'){
        this.dislike = 'https://www.flaticon.com/svg/vstatic/svg/2107/2107616.svg?token=exp=1611638176~hmac=c5331029c9417f905a16d251adad1871'
        this.like = 'https://www.flaticon.com/svg/vstatic/svg/633/633759.svg?token=exp=1611566290~hmac=adb18c3aff33a26105e6a72408673378'
      } 
      else {
        this.dislike = 'https://www.flaticon.com/svg/vstatic/svg/2107/2107811.svg?token=exp=1611638411~hmac=080d622ab8c26491007ca74a4ebe781a'
      } 
    }
  }
}
</script>

<style scoped>
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
  margin-left: 0px;
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
