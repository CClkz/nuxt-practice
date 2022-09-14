<template>
  <div>plugins</div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'PluginsPage',
  created(){
    console.log((this as any).$myInjectedFunction("plugins"));

  }
})
</script>
