<template>
    <div class="footer-contact">
        <button>sign-up now!</button>
        <div class="contact">
            <span>follow us</span>
            <img v-for="(image, index) in images" :key="index"
            :src="image.url" :alt="`${image.alt} icon`">
        </div>
    </div> 
</template>

<script>
export default {
    data: function() {
        return {
            images: [
                {
                    url: require("../assets/img/footer-facebook.png"),
                    alt: "fb"
                },
                {
                    url: require("../assets/img/footer-twitter.png"),
                    alt: "twitter"
                },
                {
                    url: require("../assets/img/footer-youtube.png"),
                    alt: "yt"
                },
                {
                    url: require("../assets/img/footer-pinterest.png"),
                    alt: "pinterest"
                },
                {
                    url: require("../assets/img/footer-periscope.png"),
                    alt: "periscope"
                },
            ]
        }
    }

}
</script>

<style lang="scss" scoped>
    .footer-contact {
        display: flex;
        justify-content: space-between;
        width: 100%;
        padding: 20px;
        background-color: #303030;

        button {
            padding: 10px;
            border: 2px solid #0282f9;
            background-color: transparent;
            text-transform: uppercase;
            color: white;
            cursor: pointer;

            &:hover {
                scale: 1.2;
            }
        }

        .contact {
            display: flex;
            align-items: center;

            span {
                color: #0282f9;
                text-transform: uppercase;
            }

            img {
                margin: 0 10px;
                cursor: pointer;

                &:hover {
                    scale: 1.1;
                }
            }
        }
    }
</style>