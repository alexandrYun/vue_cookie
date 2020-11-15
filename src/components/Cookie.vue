<template>
    <img :src="cookie" v-on:click="$emit('counterup')">
</template>

<script>
import cookie from '@/assets/oreo.png'
export default {
    data() {
        return {
            cookie
        }
    }
}
</script>

<style scoped>
    img {
        height: 400px;
    }
</style>