<template>
    <div>
        <home-header></home-header>
        <home-swiper></home-swiper>
        <div>test</div>
    </div>
</template>

<script>
import HomeHeader from './components/HomeHeader'
import HomeSwiper from './components/HomeSwiper';
export default {
    name: 'HomeCom',
    components: {
        HomeHeader,
        HomeSwiper
    }
}
</script>

<style lang="scss" scoped>
</style>