<template>
  <div>
      <h1>videos index</h1>
    <div v-for="video in videos" :key="video.id">
      <nuxt-link :to="`/videos/${video.id}`"> {{ video.name }}</nuxt-link>
      <!-- {{video.name}} -->
    </div>
  </div>
</template>

<script>
export default {
  async asyncData(context) {
    let response = await context.$axios.get(
      'https://www.getpostman.com/collections/b5d56032bd3980bc133b'
    )
    const testing = response.data.info.name
    console.warn(testing);
    // let videos = response.data.map(v => v.attributes)
    // console.warn(videos);
    console.log(response.data)
    console.warn(response.data);
    // console.warn(response.data.info);
    console.warn(response.data.info.name);  //-->working properly
    // console.warn(response.data.item);
    // console.warn(response.headers);
    // console.warn(response.data.item);
    // console.warn(response.data);
    // console.warn(response.data);
    debugger
    // return{
    //     videos
    // }

  },
  data() {
      return {
          videos:[{
              id:16,
              name: "a lkjdf dlj lad"
          },
          {
              id:1,
              name: "aadfadfaf lkjdf dlj lad"
          },
          {
              id:71,
              name: "adfadfafdfagfgfg lkdjsf j lkjdf dlj lad"
          },
          ]
      }
  },
}
</script>

<style lang="scss" scoped>
</style>
// 48:55