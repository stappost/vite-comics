<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
    data() {
        return {
            links: [
                {
                    name: 'characters',
                    active: false,
                    url: '#'
                },
                {
                    name: 'comics',
                    active: true,
                    url: '#'
                },
                {
                    name: 'movies',
                    active: false,
                    url: '#'
                },
                {
                    name: 'tv',
                    active: false,
                    url: '#'
                },
                {
                    name: 'games',
                    active: false,
                    url: '#'
                },
                {
                    name: 'collectibles',
                    active: false,
                    url: '#'
                },
                {
                    name: 'videos',
                    active: false,
                    url: '#'
                },
                {
                    name: 'fans',
                    active: false,
                    url: '#'
                },
                {
                    name: 'news',
                    active: false,
                    url: '#'
                },
                {
                    name: 'shop',
                    active: false,
                    url: '#'
                }
            ]
        }
    },
    components: {
        AppHeader,
        AppMain,
        AppFooter,
    }
}
</script>
<template lang="">
    <div>
        <AppHeader :links="links"/>
        <AppMain />
        <AppFooter :links="links"/>
    </div>
</template>
<style lang="scss">
@use './styles/generals.scss' as *;
@use './styles/partials/variabiles' as *;
</style>