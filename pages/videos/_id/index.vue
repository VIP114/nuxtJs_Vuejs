<template>
    <div>
        <h1>{{$route.params.id}} page video</h1>
        {{video.name}}
        <br/>
        <br/>
        <nuxt-link :to="`/videos/${video.id}/edit`">
            <button>Edit</button>
        </nuxt-link>
    </div>
</template>

<script>
    export default {
        props:['video']                
    }
</script>

<style lang="scss" scoped>

</style>