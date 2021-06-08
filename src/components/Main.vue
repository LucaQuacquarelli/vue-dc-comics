<template>
    <main>
        <div class="content">
            <span>current series</span>
            <div class="comics-container">
                <Comics v-for="(item, index) in items" :key="index"
                :img="item.thumb"
                :comicsTitle="item.series"/>
            </div>
        </div>
    </main>
</template>

<script>
import comics from '../data/comics'
import Comics from './Comics.vue'


export default {
  components: {
      Comics 
    },
    data: function() {
        return {
            items: comics
        }
    }
}
</script>

<style lang="scss" scoped>
    .content {
        position: relative;
        padding: 40px 20px;
        background-color: black;
        color: white;

        span {
            position:absolute;
            top: -20px;
            padding: 10px 25px;
            background-color: #0282f9;
            text-transform: uppercase;
        }

    }
</style>