<template>
  <div>
    <div class="mb-5 pa-10">
      <h5 class="home-title">Popular Item in the market</h5>
      <h2 class='home-subtitle'>Best <span class="subtitle-item">Sellers</span></h2>
    </div>
    <v-sheet
      class="mx-auto"
      elevation="1"
    >
      <v-slide-group
        v-model="model"
        class="pa-4"
        active-class="success"
        show-arrows
        next-icon="mdi-arrow-right"
        prev-icon="mdi-arrow-left"
      >
        <v-slide-item
          v-slot="{ active, toggle }"
          width="300"
          class="mr-2"
        >
          <v-hover v-slot="{ hover }">
            <v-card
                  class="mx-auto"
                  width="300"
                  flat
              >
                  <v-img
                   :aspect-ratio="16/9"
                   :src="getImageUrl('product1.png')"

                  >
                     <v-expand-transition>
                        <div
                          v-if="hover"
                          class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal text-h2 white--text"
                          style="height: 40%;"
                       >
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-magnify</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class='ma-1'>
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-cart</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-heart</v-icon>
                      </v-btn>
                    </v-hover>
                        </div>
                     </v-expand-transition>
                  </v-img>
                  <div class="text-center mt-2">
                    <h5 class='home-title'>Accessories</h5>
                    <h3 class="font-weight-medium ma-1" :class="hover ? 'primary--text' : ''">Quartz Belt Watch</h3>
                    <h4 class="home-cart-price">$150.00</h4>
                  </div>
                </v-card>
            </v-hover>
        </v-slide-item>
        <v-slide-item
          v-slot="{ active, toggle }"
          width="300"
          class="mr-2"
        >
          <v-hover v-slot="{ hover }">
            <v-card
                  class="mx-auto"
                  width="300"
                  flat
              >
                  <v-img
                   :aspect-ratio="16/9"
                   :src="getImageUrl('product2.png')"

                  >
                     <v-expand-transition>
                        <div
                          v-if="hover"
                          class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal text-h2 white--text"
                          style="height: 40%;"
                       >
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-magnify</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class='ma-1'>
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-cart</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-heart</v-icon>
                      </v-btn>
                    </v-hover>
                        </div>
                     </v-expand-transition>
                  </v-img>
                  <div class="text-center mt-2">
                    <h5 class='home-title'>Accessories</h5>
                    <h3 class="font-weight-medium ma-1" :class="hover ? 'primary--text' : ''">Quartz Belt Watch</h3>
                    <h4 class="home-cart-price">$150.00</h4>
                  </div>
                </v-card>
            </v-hover>
        </v-slide-item>
        <v-slide-item
          v-slot="{ active, toggle }"
          width="300"
          class="mr-2"
        >
          <v-hover v-slot="{ hover }">
            <v-card
                  class="mx-auto"
                  width="300"
                  flat
              >
                  <v-img
                   :aspect-ratio="16/9"
                   :src="getImageUrl('product3.png')"

                  >
                     <v-expand-transition>
                        <div
                          v-if="hover"
                          class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal text-h2 white--text"
                          style="height: 40%;"
                       >
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-magnify</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class='ma-1'>
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-cart</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-heart</v-icon>
                      </v-btn>
                    </v-hover>
                        </div>
                     </v-expand-transition>
                  </v-img>
                  <div class="text-center mt-2">
                    <h5 class='home-title'>Accessories</h5>
                    <h3 class="font-weight-medium ma-1" :class="hover ? 'primary--text' : ''">Quartz Belt Watch</h3>
                    <h4 class="home-cart-price">$150.00</h4>
                  </div>
                </v-card>
            </v-hover>
        </v-slide-item>
        <v-slide-item
          v-slot="{ active, toggle }"
          width="300"
          class="mr-2"
        >
          <v-hover v-slot="{ hover }">
            <v-card
                  class="mx-auto"
                  width="300"
                  flat
              >
                  <v-img
                   :aspect-ratio="16/9"
                   :src="getImageUrl('product4.png')"

                  >
                     <v-expand-transition>
                        <div
                          v-if="hover"
                          class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal text-h2 white--text"
                          style="height: 40%;"
                       >
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-magnify</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class='ma-1'>
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-cart</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-heart</v-icon>
                      </v-btn>
                    </v-hover>
                        </div>
                     </v-expand-transition>
                  </v-img>
                  <div class="text-center mt-2">
                    <h5 class='home-title'>Accessories</h5>
                    <h3 class="font-weight-medium ma-1" :class="hover ? 'primary--text' : ''">Quartz Belt Watch</h3>
                    <h4 class="home-cart-price">$150.00</h4>
                  </div>
                </v-card>
            </v-hover>
        </v-slide-item>
        <v-slide-item
          v-slot="{ active, toggle }"
          width="300"          
          class="mr-2"
        >
          <v-hover v-slot="{ hover }">
            <v-card
                  class="mx-auto"
                  width="300"
                  flat
              >
                  <v-img
                   :aspect-ratio="16/9"
                   :src="getImageUrl('product5.png')"

                  >
                     <v-expand-transition>
                        <div
                          v-if="hover"
                          class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal text-h2 white--text"
                          style="height: 40%;"
                       >
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-magnify</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class='ma-1'>
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-cart</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-heart</v-icon>
                      </v-btn>
                    </v-hover>
                        </div>
                     </v-expand-transition>
                  </v-img>
                  <div class="text-center mt-2">
                    <h5 class='home-title'>Accessories</h5>
                    <h3 class="font-weight-medium ma-1" :class="hover ? 'primary--text' : ''">Quartz Belt Watch</h3>
                    <h4 class="home-cart-price">$150.00</h4>
                  </div>
                </v-card>
            </v-hover>
        </v-slide-item>
        <v-slide-item
          v-slot="{ active, toggle }"
          width="300"
          class="mr-2"
        >
          <v-hover v-slot="{ hover }">
            <v-card
                  class="mx-auto"
                  width="300"
                  flat
              >
                  <v-img
                   :aspect-ratio="16/9"
                   :src="getImageUrl('product6.png')"

                  >
                     <v-expand-transition>
                        <div
                          v-if="hover"
                          class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal text-h2 white--text"
                          style="height: 40%;"
                       >
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-magnify</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class='ma-1'>
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-cart</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-heart</v-icon>
                      </v-btn>
                    </v-hover>
                        </div>
                     </v-expand-transition>
                  </v-img>
                  <div class="text-center mt-2">
                    <h5 class='home-title'>Accessories</h5>
                    <h3 class="font-weight-medium ma-1" :class="hover ? 'primary--text' : ''">Quartz Belt Watch</h3>
                    <h4 class="home-cart-price">$150.00</h4>
                  </div>
                </v-card>
            </v-hover>
        </v-slide-item>
        <v-slide-item
          v-slot="{ active, toggle }"
          width="300"
          class="mr-2"
        >
          <v-hover v-slot="{ hover }">
            <v-card
                  class="mx-auto"
                  width="300"
                  flat
              >
                  <v-img
                   :aspect-ratio="16/9"
                   :src="getImageUrl('product7.png')"

                  >
                     <v-expand-transition>
                        <div
                          v-if="hover"
                          class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal text-h2 white--text"
                          style="height: 40%;"
                       >
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-magnify</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class='ma-1'>
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-cart</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-heart</v-icon>
                      </v-btn>
                    </v-hover>
                        </div>
                     </v-expand-transition>
                  </v-img>
                  <div class="text-center mt-2">
                    <h5 class='home-title'>Accessories</h5>
                    <h3 class="font-weight-medium ma-1" :class="hover ? 'primary--text' : ''">Quartz Belt Watch</h3>
                    <h4 class="home-cart-price">$150.00</h4>
                  </div>
                </v-card>
            </v-hover>
        </v-slide-item>
        <v-slide-item
          v-slot="{ active, toggle }"
          width="300"          
          class="mr-2"
        >
          <v-hover v-slot="{ hover }">
            <v-card
                  class="mx-auto"
                  width="300"
                  flat
              >
                  <v-img
                   :aspect-ratio="16/9"
                   :src="getImageUrl('product8.png')"

                  >
                     <v-expand-transition>
                        <div
                          v-if="hover"
                          class="d-flex transition-fast-in-fast-out white darken-2 v-card--reveal text-h2 white--text"
                          style="height: 40%;"
                       >
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-magnify</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class='ma-1'>
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-cart</v-icon>
                      </v-btn>
                    </v-hover>
                        <v-hover v-slot="{ hover }">
                      <v-btn small fab :color="hover ? 'white' : 'primary'" class="ma-1">
                        <v-icon :color="hover ? 'primary' : 'white'">mdi-heart</v-icon>
                      </v-btn>
                    </v-hover>
                        </div>
                     </v-expand-transition>
                  </v-img>
                  <div class="text-center mt-2">
                    <h5 class='home-title'>Accessories</h5>
                    <h3 class="font-weight-medium ma-1" :class="hover ? 'primary--text' : ''">Quartz Belt Watch</h3>
                    <h4 class="home-cart-price">$150.00</h4>
                  </div>
                </v-card>
            </v-hover>
        </v-slide-item>
      </v-slide-group>
    </v-sheet>
  </div>
</template>


<script>
  export default {
    data: () => ({
      model: null,
    }),
        methods: {
      getImageUrl(img){
        return require(`@/assets/images/product/${img}`)
      }
    }
  }
</script>

<style>
.v-card--reveal {
  align-items: center;
  bottom: 0;
  justify-content: center;
  opacity: 0.9;
  position: absolute;
  width: 100%;
}
.home-title{
  color: grey;
  font-weight: 100;
  font-size: 16px;
}
.home-subtitle{
  color: black;
  font-size: 36px;
  font-family: Ubuntu;
}
.subtitle-item{
  padding: 5px;
  border-bottom: 2px solid blue;
}
</style>