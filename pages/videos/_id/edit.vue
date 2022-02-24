<template>
    <div>
        <!-- <h2>editing {{$route.params.id}}</h2> -->
        <h2>editing {{video.name}}</h2>
        <br/>
        <br/>
        <nuxt-link :to="`/videos/${video.id}`">
            <button>Go back to Show</button>
        </nuxt-link>
        <br/>
        <br/>
        <nuxt-link :to="`/videos/`">
            <button>Go To Video Page</button>
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