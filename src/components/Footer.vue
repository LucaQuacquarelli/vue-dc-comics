<template>
  <footer>
      <div class="footer-link">
          <div class="list">
              <h4>DC Comics</h4>
              <ul>
                  <li><a href="#characters">Characters</a></li>
                  <li><a href="#comics">Comics</a></li>
                  <li><a href="#movies">Movies</a></li>
                  <li><a href="#tv">Tv</a></li>
                  <li><a href="#games">Games</a></li>
                  <li><a href="#videos">Videos</a></li>
                  <li><a href="#news">News</a></li>
              </ul>
              <h4>Shop</h4>
              <ul>
                  <li><a href="#shop-dc">Shop DC</a></li>
                  <li><a href="#shop-dc-collectables">Shop DC Collectables</a></li>
              </ul>
          </div>
          <div class="list">
              <h4>DC Comics</h4>
              <ul>
                  <li><a href="#characters">Characters</a></li>
                  <li><a href="#comics">Comics</a></li>
                  <li><a href="#movies">Movies</a></li>
                  <li><a href="#tv">Tv</a></li>
                  <li><a href="#games">Games</a></li>
                  <li><a href="#videos">Videos</a></li>
                  <li><a href="#news">News</a></li>
              </ul>
          </div>
          <div class="list">
              <h4>DC Comics</h4>
              <ul>
                  <li><a href="#characters">Characters</a></li>
                  <li><a href="#comics">Comics</a></li>
                  <li><a href="#movies">Movies</a></li>
                  <li><a href="#tv">Tv</a></li>
                  <li><a href="#games">Games</a></li>
                  <li><a href="#videos">Videos</a></li>
                  <li><a href="#news">News</a></li>
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