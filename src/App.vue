<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbo from './components/AppJumbo.vue';
import AppCards from './components/AppCards.vue';
import AppPrograms from './components/AppPrograms.vue';
import AppCarousel from './components/AppCarousel.vue';
import AppFooter from './components/AppFooter.vue';


export default {
    components: {
        AppHeader,
        AppJumbo,
        AppCards,
        AppPrograms,
        AppCarousel,
        AppFooter,
    },
    data() {
        return {

        }
    }
}
</script>

<template>
    <AppHeader />
    <AppJumbo />
    <AppCards />
    <AppPrograms />
    <AppCarousel />
    <AppFooter />
</template>

<style scoped lang="scss"></style>
