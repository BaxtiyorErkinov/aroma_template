<template>
	<div>
		<v-card>
	      <v-item-group
	        multiple
	      >
	        <v-row>
	          <v-col
	            cols="12"
	            md="2"
	            sm="4"
	            class="px-0 py-0"
	          >
	            <v-hover v-slot="{ hover }">
	            <v-item v-slot="{ active, toggle }">
	              <v-img
	                :src="getImg(`ins-1.jpg`)"
	                height="200"
	                width="350"
	                class="text-right pa-2"
	                @click="toggle"
	                :class="hover ? 'cont' : 'disabled'"
	              >
	                <v-btn
	                  icon
	                  dark
	                >
	                  <v-icon>
	                    {{ active ? 'mdi-heart' : 'mdi-heart-outline' }}
	                  </v-icon>
	                </v-btn>
	              </v-img>
	            </v-item>
	          	</v-hover>
	          </v-col>
	          	          <v-col
	            cols="12"
	            md="2"
	            sm="4"
	            class="px-0 py-0"
	          >
	            <v-hover v-slot="{ hover }">

	            <v-item v-slot="{ active, toggle }">
	              <v-img
	                :src="getImg(`ins-2.jpg`)"
	                height="200"
	                width="350"
	                class="text-right pa-2"
	                @click="toggle"
	                :class="hover ? 'cont' : 'disabled'"

	              >
	                <v-btn
	                  icon
	                  dark
	                >
	                  <v-icon>
	                    {{ active ? 'mdi-heart' : 'mdi-heart-outline' }}
	                  </v-icon>
	                </v-btn>
	              </v-img>
	            </v-item>
	        </v-hover>
	          </v-col>
	          	          <v-col
	            cols="12"
	            md="2"
	            sm="4"
	            class="px-0 py-0"
	          >
	            <v-hover v-slot="{ hover }">

	            <v-item v-slot="{ active, toggle }">
	              <v-img
	                :src="getImg(`ins-3.jpg`)"
	                height="200"
	                width="350"
	                class="text-right pa-2"
	                @click="toggle"
	                :class="hover ? 'cont' : 'disabled'"

	              >
	                <v-btn
	                  icon
	                  dark
	                >
	                  <v-icon>
	                    {{ active ? 'mdi-heart' : 'mdi-heart-outline' }}
	                  </v-icon>
	                </v-btn>
	              </v-img>
	            </v-item>
	        </v-hover>
	          </v-col>
	          <div class="pos">
	      		<v-btn color="#fff" x-large><span class="caption font">More Instagram</span><v-icon small class="ml-1">mdi-instagram</v-icon></v-btn>
	      	</div>
	          <v-col
	            cols="12"
	            md="2"
	            sm='4'
	            class="px-0 py-0"
	          >
	            <v-hover v-slot="{ hover }">
	            <v-item v-slot="{ active, toggle }">
	              <v-img
	                :src="getImg(`ins-4.jpg`)"
	                height="200"
	                width="350"
	                class="text-right pa-2"
	                @click="toggle"
	                :class="hover ? 'cont' : 'disabled'"

	              >
	                <v-btn
	                  icon
	                  dark
	                >
	                  <v-icon>
	                    {{ active ? 'mdi-heart' : 'mdi-heart-outline' }}
	                  </v-icon>
	                </v-btn>
	              </v-img>
	            </v-item>
	        </v-hover>
	          </v-col>
	          	          <v-col
	            cols="12"
	            md="2"
	            sm="4"
	            class="px-0 py-0"
	          >
	            <v-hover v-slot="{ hover }">

	            <v-item v-slot="{ active, toggle }">
	              <v-img
	                :src="getImg(`ins-5.jpg`)"
	                height="200"
	                width="350"
	                class="text-right pa-2"
	                @click="toggle"
	                :class="hover ? 'cont' : 'disabled'"

	              >
	                <v-btn
	                  icon
	                  dark
	                >
	                  <v-icon>
	                    {{ active ? 'mdi-heart' : 'mdi-heart-outline' }}
	                  </v-icon>
	                </v-btn>
	              </v-img>
	            </v-item>
	        </v-hover>
	          </v-col>
	          	          <v-col
	            cols="12"
	            md="2"
	            sm="4"
	            class="px-0 py-0"
	          >
	            <v-hover v-slot="{ hover }">
	            <v-item v-slot="{ active, toggle }">
	              <v-img
	                :src="getImg(`ins-6.jpg`)"
	                height="200"
	                width="350"
	                class="text-right pa-2"
	                @click="toggle"
	                :class="hover ? 'cont' : 'disabled'"

	              >
	                <v-btn
	                  icon
	                  dark
	                >
	                  <v-icon>
	                    {{ active ? 'mdi-heart' : 'mdi-heart-outline' }}
	                  </v-icon>
	                </v-btn>
	              </v-img>
	            </v-item>
	        </v-hover>
	          </v-col>
	        </v-row>
	      </v-item-group>
  	</v-card>
	</div>
</template>

<script>
	export default{
		data(){
			return{
				photos: [
					{
						id: 1,
						img: 'ins-1.jpg'
					},
					{
						id: 2,
						img: 'ins-2.jpg'
					},
					{
						id: 3,
						img: 'ins-3.jpg'
					},
					{
						id: 4,
						img: 'ins-4.jpg'
					},
					{
						id: 5,
						img: 'ins-5.jpg'
					},
					{
						id: 6,
						img: 'ins-6.jpg'
					}
				]
			}
		},
		methods: {
			getImg(img){
				return require(`~/assets/images/instagram/${img}`)
			}
		}
	}
</script>
<style scoped>
	.pos{
		position: absolute;
		top: 30%;
		right: 45%;
		z-index: 2000;
	}
	.font{
		font-family: monospace;
	}
@media only screen 
  and (min-device-width: 768px) 
  and (max-device-width: 1024px){
  		.pos{
		position: absolute;
		top: 43%;
		right: 38%;
		z-index: 1000;
	}
  }
@media only screen 
  and (min-device-width: 360px) 
  and (max-device-width: 640px){
  		.pos{
		position: absolute;
		top: 32%;
		right: 30%;
		z-index: 1000;
	}
  }
.cont{
	transform: scale(1.03);
	z-index: 1000;
	transition: all .5s;
}
.disabled{
	transition: all .5s;
}
</style>