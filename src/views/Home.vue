<template>
  <div class="home">
    <div class="d-flex justify-content-center">
      <bot-list />
    </div>
    <hr />
    
    <div class="my-5 mx-auto">
      <img src="../assets/shibai-logo.png" title="ShibAI logo" />
    </div>

    <div>
      <h1>Welcome to the ShibAI UI</h1>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

import BotList from '@/components/BotList.vue';

export default defineComponent({
  name: 'Home',
  components: { BotList },
});
</script>

<style lang="scss" scoped>
.home {
  margin-top: 1.5em;
}
.logo-svg {
  -webkit-mask: url(../assets/shibai-logo-mask.svg) no-repeat center;
  -webkit-mask-size: 240px 240px;
  mask: url(../assets/shibai-logo-mask.svg) no-repeat center;
  mask-size: contain;
  width: 250px;
  height: 250px;
}
</style>
