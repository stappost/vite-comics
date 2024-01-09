<script>
export default {
    name: "AppHeader",
    props: {
        links: Array
    },
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


        li {
            padding: 50px 10px;

            a {
                text-decoration: none;
                color: #000;
                font-size: 13px;
                text-transform: uppercase;
                padding-bottom: 50px;
                font-weight: 600;

                &:hover {
                    color: $primary;
                    border-bottom: 5px solid $primary;
                }
            }

            .active {
                color: $primary;
                border-bottom: 5px solid $primary;
            }

        }
    }
}
</style>