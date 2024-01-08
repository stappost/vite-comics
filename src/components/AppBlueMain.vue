<script>
export default {
    name: "AppBlueMain",
    data() {
        return {
            logos: [
                {
                    src: "./src/assets/img/buy-comics-digital-comics.png",
                    item: "Digital comics",
                    link: "#"
                },
                {
                    src: "./src/assets/img/buy-comics-merchandise.png",
                    item: "dc merchandise",
                    link: "#"
                },
                {
                    src: "./src/assets/img/buy-comics-shop-locator.png",
                    item: "subscription",
                    link: "#"
                },
                {
                    src: "./src/assets/img/buy-comics-subscriptions.png",
                    item: "comic shop locator",
                    link: "#"
                },
                {
                    src: "./src/assets/img/buy-dc-power-visa.svg",
                    item: "dc power visa",
                    link: "#"
                }
            ]
        }
    }

}
</script>
<template lang="">
    <div class="bg_blue">
        <div class="container">
            <ul>
                <li v-for="(item, index) in logos">
                    <a href="item.link">
                        <img :src="item.src" :alt="item.item">
                        <span>
                            {{ item.item }}
                        </span>
                    </a>
                    
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../styles/partials/variabiles' as *;

.bg_blue {
    background-color: $primary;

    ul {
        display: flex;
        list-style: none;
        align-items: center;
        width: 100%;
        padding: 30px 0;

        li {
            width: calc(100% / 5);

            a {
                text-decoration: none;
                color: white;

                display: flex;
                align-items: center;

                img {
                    height: 50px;
                    margin: 0 10px;
                }

                span {
                    text-transform: uppercase;
                }
            }
        }


    }
}
</style>