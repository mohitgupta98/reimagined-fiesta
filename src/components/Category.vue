<template>
  <div id="rectangle">
    <div style="margin-left:0px;">
    <h2 style="font-family: Georgia, Helvetica, sans-serif; font-weight:bold; margin-bottom: 30px; border-bottom: solid; padding-bottom: 20px">Category</h2>
    <div>
      <p class="shift">Sports</p>
      <p class="shift">Politics</p>
      <p class="shift">India</p>
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
  position: fixed;
  top:100px;
  left:25px;
  width: 263px;
  height: 600px;
  background: rgb(235, 232, 232);
  border-radius: 10px;
}
.shift{
  left:0px;
  font-family: Georgia, Helvetica, sans-serif;
  font-weight:bold;
  font-size:120%;
}
</style>
