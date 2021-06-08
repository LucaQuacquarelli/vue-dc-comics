<template>
    <div class="comics">
        <div class="cover">
            <img :src="img" alt="">
        </div>
        <span>{{comicsTitle}}</span>
    </div>
</template>

<script>
export default {
    props: {
        img: String,
        comicsTitle: String
    }
}
</script>

<style lang="scss">
    .comics-container {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        
        .comics {
            display: flex;
            flex-direction: column;
            margin: 20px;
            

            .cover {
                width: 150px;
                height: 150px;

                img {
                    width: 100%;
                    height: 100%;
                }
            
            }

            span {
                width: 150px;
                margin: 10px 0;
            }
        }
    }
</style>