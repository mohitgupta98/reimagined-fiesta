<template>
<div>
<div id="rectangle">
<p>advertisement</p>
<img src="{{}}" alt="">
</div>

<div id="rectangle_two">
<p>advertisement</p>
<img src="{{}}" alt="">
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
  width: 263px;
  height: 263px;
  background: rgb(235, 232, 232);
  margin-left: 70px;
  margin-bottom: 20px;
  border-radius: 10px;
}
#rectangle_two{
  position: fixed;
  top: 100px;
  width: 263px;
  height: 263px;
  background: rgb(235, 232, 232);
  margin-left: 70px;
  margin-bottom: 20px;
  border-radius: 10px;
  margin-top: 320px;
}
</style>
