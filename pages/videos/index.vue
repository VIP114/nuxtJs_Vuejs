<template>
    <div>
        <div v-for="video in videos" :key="video.id">
            {{video.name}}
        </div>
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
    }
</script>

<style lang="scss" scoped>

</style>