<template>
  <header>
      <section class="left">
          <a href="/">
            <img src="../assets/images/dc-logo.png" alt="">
          </a>
      </section>
      <section class="right">
          <ul>
              <li v-for="(element, index) in menu" :key="index"><a href="">{{ element }}</a></li>
          </ul>
      </section>
  </header>
</template>

<script>

export default {
    name: "Header",
    data: function() {
        return {
            menu: [
                "characters",
                "comics",
                "movies",
                "tv",
                "games",
                "collectables",
                "videos",
                "fans",
                "news",
                "shop"
            ]
        }
    }
}

</script>

<style lang="scss" scope>

    @import "../style/Color.scss";
    header {
        display: flex;
        width: 70%;
        height: 80px;
        margin: auto;

    // sezione di sinistra

        .left {
            display: flex;
            width: 15%;
            height: 100%;

            a {
                margin: auto 0;

                img {
                width: 50%;
                }
                
            }

            
        }

    // sezione di destra 

        .right {
        display: flex;
        width: 85%;
        height: 100%;
        align-items: center;
        justify-content: flex-end;

            ul {
                display: flex;
                height: 100%;
                list-style: none;
            }
            li {
                
                display: flex;
                margin: auto 8px;
                font-size: 10px;
                text-transform: uppercase;
                height: 100%;

                &:hover {
                    border-bottom: 3px solid $logo-color;

                    & a {
                        color: $logo-color;
                    }
                }
                
            }
            a {
                text-decoration: none;
                color: black;
                margin: auto;
                font-weight: 700;
            }
        }
    }
    
</style>