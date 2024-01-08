<script>
export default {
    name: "AppHeader",
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
    }
}
</script>
<template >
    <header>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="logo">
                        <img src="../assets/img/dc-logo.png" alt="logo">
                    </div>
                    <div class="menu">
                        <ul>
                            <li v-for="(link, index) in links" key="index">
                                <a href="link.url" :class="link.active ? 'active' : ''">
                                    {{ link.name }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </header>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variabiles' as *;

header {
    height: 100px;

    .logo {
        height: 80%;
        margin: 10px 0;

        img {
            height: 100%;
        }
    }

    .col-12 {
        display: flex;
        justify-content: space-between;
    }

    ul {
        display: flex;
        flex-wrap: wrap;
        list-style: none;
        align-items: center;
        height: 100px;

        li {
            padding: 10px;

            a {
                text-decoration: none;
                color: #000;

            }

            .active {
                color: $primary;
            }
        }
    }
}
</style>