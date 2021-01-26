<template>
<div id="notification_page">
  <div>
    <Category></Category>
  </div>
  <div>
  <h2>My Notifications</h2>
  <Notification></Notification>
  <Notification></Notification>
  <FollowRequest></FollowRequest>
  <Notification></Notification>
  <Notification></Notification>
  <FollowRequest></FollowRequest>
  <Notification></Notification>
</div>
<div>
  <Advertisement></Advertisement>
</div>
</div>
</template>

<script>
import Advertisement from '../components/Advertisement.vue'
import Category from '../components/Category.vue'
import FollowRequest from '../components/FollowRequest.vue'
import Notification from '../components/Notification.vue'
export default {
  components: { Notification, Category, Advertisement, FollowRequest }

}
</script>

<style scoped>
#notification_page{
  display: flex;
}
</style>
