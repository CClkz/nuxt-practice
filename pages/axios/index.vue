<template>
  <div>axios</div>
</template>

<script lang="ts">
import Vue from 'vue'
import axios from '@nuxtjs/axios'

export default Vue.extend({
  name: 'AxiosPage',
//   promise
  //   asyncData({ params, $axios }) {
  //     return $axios.get(`https://my-api/posts/${params.id}`).then((res: any) => {
  //       return { title: res.data.title }
  //     })
  //   },
//   async await
  async asyncData({ params, $axios }) {
    const res = await $axios.get(`https://my-api/posts/${params.id}`)
    return { title: res.data.title }
  },
})
</script>