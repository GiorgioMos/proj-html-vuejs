<script>
import AppHeader from './components/AppHeader.vue';
import AppJumbo from './components/AppJumbo.vue';
import AppFooter from './components/AppFooter.vue';
import AppCards from './components/AppCards.vue';


export default {
    components: {
        AppHeader,
        AppJumbo,
        AppCards,
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
    <AppFooter />
</template>

<style scoped lang="scss"></style>
