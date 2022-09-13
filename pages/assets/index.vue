<template>
  <div>
    <p class="assets">assets<img src="~/assets/favicon.png"></p>
    <p>static<img src="/favicon.ico"></p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'AssetPage',
})
</script>
<style>
/* .assets{
  width: 200px;
  height: 200px;
  background: url(/favicon.ico);
} */
</style>
