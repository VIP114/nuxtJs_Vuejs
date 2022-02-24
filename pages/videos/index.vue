<template>
    <div>
        <div v-for="video in videos" :key="video.id">
            {{video.name}}
        </div>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style lang="scss" scoped>

</style>