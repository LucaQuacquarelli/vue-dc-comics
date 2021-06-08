<template>
  <footer>
      <div class="footer-link">
          <div class="list">
              <h4>DC Comics</h4>
              <ul>
                  <li v-for="(link, index) in linkComics" :key="index"><a :href="`#${link.url}`">{{link.linkName}}</a></li>
              </ul>
              <h4>Shop</h4>
              <ul>
                  <li v-for="(link, index) in linkShop" :key="index"><a :href="`#${link.url}`">{{link.linkName}}</a></li>
              </ul>
          </div>
          <div class="list">
              <h4>DC</h4>
              <ul>
                  <li v-for="(link, index) in linkDc" :key="index"><a :href="`#${link.url}`">{{link.linkName}}</a></li>
              </ul>
          </div>
          <div class="list">
              <h4>Sites</h4>
              <ul>
                  <li v-for="(link, index) in linkSites" :key="index"><a :href="`#${link.url}`">{{link.linkName}}</a></li>
              </ul>
          </div>
      </div>
      <div class="footer-logo">
          <img src="../assets/img/dc-logo-bg.png" alt="dc logo bg">
      </div>
  </footer>
</template>

<script>
export default {
    data: function() {
        return {
            linkComics: [
                {
                    url: "characters",
                    linkName: "Characters"
                },
                {
                    url: "comics",
                    linkName: "Comics"
                },
                {
                    url: "movies",
                    linkName: "Movies"
                },
                {
                    url: "tv",
                    linkName: "Tv"
                },
                {
                    url: "games",
                    linkName: "Games"
                },
                {
                    url: "videos",
                    linkName: "Videos"
                },
                {
                    url: "news",
                    linkName: "News"
                },
            ],
            linkShop: [
                {
                    url: "shop-dc",
                    linkName: "Shop DC"
                },
                {
                    url: "shop-dc-collectibles",
                    linkName: "Shop DC Collectibles"
                }
            ],
            linkDc: [
                {
                    url: "term-of-use",
                    linkName: "Term Of Use"
                },
                {
                    url: "privacy-policy-new",
                    linkName: "Privacy Policy (New)"
                },
                {
                    url: "ad-choices",
                    linkName: "Ad Choices"
                },
                {
                    url: "advertising",
                    linkName: "Advertising"
                },
                {
                    url: "jobs",
                    linkName: "Jobs"
                },
                {
                    url: "subscriptions",
                    linkName: "Subscriptions"
                },
                {
                    url: "talent-workshop",
                    linkName: "Talent Workshop"
                },
                {
                    url: "cpsc-certificates",
                    linkName: "CPSC Certificates"
                },
                {
                    url: "ratings",
                    linkName: "Ratings"
                },
                {
                    url: "shop-helps",
                    linkName: "Shop Help"
                },
                {
                    url: "contact-us",
                    linkName: "Contact Us"
                }
            ],
            linkSites: [
                {
                    url: "dc",
                    linkName: "DC"
                },
                {
                    url: "mad-magazine",
                    linkName: "MAD Magazine"
                },
                {
                    url: "dc-kids",
                    linkName: "DC Kids"
                },
                {
                    url: "dc-universe",
                    linkName: "DC Universe"
                },
                {
                    url: "dc-power-visa",
                    linkName: "DC Power Visa"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    footer {
        display: flex;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;

        .footer-link {
            display: flex;
            width: 50%;
            height: 100%;
            padding: 30px 20px;
            
            .list {
                margin-right: 30px;

                h4 {
                    color: white;
                    text-transform: uppercase;
                }

                ul {
                    margin-bottom: 30px;
                    
                    li {
                        list-style: none;

                        a {
                            font-size: 12px;
                            text-decoration: none;
                            color: #6a697a;

                            &:hover {
                                text-decoration: underline;
                            }
                        }

                    }

                }

            }

        }

        .footer-logo {
            display: flex;
            justify-content: center;
            align-items: center;
            width: 50%;
            overflow: hidden;

            img {
                width: 50%;
                scale: 1.5;
            }

        }
    }
</style>