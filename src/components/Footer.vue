<template>
  <div class="footer">
    
    <div class="left"><a target="_blank" href="https://icons8.com/icon/3Y6IMdWhMqqx/game-controller">Game Controller</a> icon by <a target="_blank" href="https://icons8.com">Icons8</a></div> 
    <div class="right">Reach me at <a href="mailto:markhoitsma@gmail.com">markhoitsma@gmail.com</a> or <router-link to="/contact">through here</router-link></div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Footer"
});
</script>

<style scoped lang="less">

@import '../css/variables.less';

.footer {
  background-color: @bodyBgColor;
  width: 100%;
  font-size: 0.8em;
  opacity: 0.7;
  padding-bottom: 30px;
}

.left, .right {
    padding-top: 10px;
    text-align: center;
  }

@media only screen and (min-width: 620px){

  .footer {
    padding: 0;
  }

  .left, .right {
    padding: 20px;
  }

  .left {
    float: left;
  }

  .right {
    float:right;
  }
}
</style>