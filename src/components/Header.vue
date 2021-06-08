<template>
  <header>
      <div class="logo-container">
          <a href="#">
              <img src="../assets/img/dc-logo.png" alt="dc logo">
          </a>
      </div>
      <nav>
          <ul>
              <li v-for="(link, index) in links" 
              :key="index" 
              :class="index == activeIndex ? 'active': ''"
              @click="setActive(index)">
                <a :href="link.url">{{link.name}}</a>
              </li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
    data: function () {
        return {
            links: [
                {
                    name: "Characters",
                    url: "#characters"
                },
                {
                    name: "Comics",
                    url: "#comics"
                },
                {
                    name: "Movies",
                    url: "#movies"
                },
                {
                    name: "Tv",
                    url: "#tv"
                },
                {
                    name: "Games",
                    url: "#games"
                },
                {
                    name: "Collectibles",
                    url: "#collectibles"
                },
                {
                    name: "Videos",
                    url: "#videos"
                },
                {
                    name: "Fans",
                    url: "#fans"
                },
                {
                    name: "News",
                    url: "#news"
                },
                {
                    name: "Shop",
                    url: "#shop"
                },
            ],
            activeIndex: 1
        }
    },
    methods: {
        setActive: function(newIndex) {
            this.activeIndex = newIndex;
        },
    }
}
</script>

<style lang="scss" scoped>
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 20px;
        padding-top: 5px;
        padding-bottom: 0;

        img {
            width: 70%;
        }
        
        nav {

            ul {
                display: flex;

                li {
                    margin: 0 10px;
                    padding: 30px 0;
                    list-style: none;

                    a {
                        text-decoration: none;
                        text-transform: uppercase;
                        color: black;
                    }

                    &:hover,
                    &.active  {
                        border-bottom: 3px solid #0282f9;
                    }

                    &:hover a,
                    &.active a {
                        color: #0282f9;
                    }

                }

            }
            
        }

    }
</style>