<template>
    <section>
        <div v-for="(shop, index) in shops" :key="index" class="shop">
            <img :src="shop.imgUrl" :alt="`${shop.imgAlt} icon`">
            <a :href="`#${shop.linkUrl}`">{{shop.linkName}}</a>
        </div>
    </section>
</template>

<script>
export default {
    data: function() {
        return {
            shops: [
                {
                    imgUrl: require("../assets/img/buy-comics-digital-comics.png"),
                    imgAlt: "digital comics",
                    linkUrl: "digital-comics",
                    linkName: "digital comics"
                },
                {
                    imgUrl: require("../assets/img/buy-comics-merchandise.png"),
                    imgAlt: "merchandise",
                    linkUrl: "merchandise",
                    linkName: "merchandise"
                },
                {
                    imgUrl: require("../assets/img/buy-comics-subscriptions.png"),
                    imgAlt: "subscription",
                    linkUrl: "subscriptions",
                    linkName: "subscriptions"
                },
                {
                    imgUrl: require("../assets/img/buy-comics-shop-locator.png"),
                    imgAlt: "comic shop locator",
                    linkUrl: "comic-shop-locator",
                    linkName: "comic shop locator"
                },
                {
                    imgUrl: require("../assets/img/buy-dc-power-visa.svg"),
                    imgAlt: "dc power visa",
                    linkUrl: "dc-power-visa",
                    linkName: "dc power visa"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    section {
        display: flex;
        justify-content: space-between;
        padding: 50px;
        background-color: #0282f9;

        .shop {
            display: flex;
            align-items: center;

            img {
                height: 50px;
            }

            a {
                margin: 0 15px;
                text-transform: uppercase;
                color: white;
                text-decoration: none;

                &:hover {
                    text-decoration: underline;
                    scale: 1.1;
                }
            }

        }

    }
</style>