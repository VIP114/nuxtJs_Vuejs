<template>
    <div>
        <nuxt-child :video="video"/>
    </div>
</template>

<script>
    export default {
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
        computed: {
            video() {
                 return this.videos.find(v => v.id == this.$route.params.id)
            }
        },
    }
</script>

<style lang="scss" scoped>

</style>