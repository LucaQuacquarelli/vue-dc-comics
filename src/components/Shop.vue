<template>
    <section>
        <div class="shop">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="subscription icon">
            <a href="#digital-comics">digital comics</a>
        </div>
        <div class="shop">
            <img src="../assets/img/buy-comics-merchandise.png" alt="subscription icon">
            <a href="#dc-merchandise">dc merchandise</a>
        </div>
        <div class="shop">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="subscription icon">
            <a href="#subscription">subscription</a>
        </div>
        <div class="shop">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="shop-locator icon">
            <a href="#comic-shop-locator">comic shop locator</a>
        </div>
        <div class="shop">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="visa icon">
            <a href="#dc-power-visa">dc power visa</a>
        </div>
    </section>
</template>

<script>
export default {

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