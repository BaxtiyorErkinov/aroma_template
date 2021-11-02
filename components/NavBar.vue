<template>
	<div>
		<v-app-bar fixed scroll-threshold color="#fff" class="pl-15 pl-md-0">
					<div class="navigation align-center">
						<v-row>
							<v-col cols="2" width="100" class="align-self-center">
								<div class="items justify-center text-center"><img src="@/assets/images/logo.png" /></div>
							</v-col>
							<v-col cols="8" class="d-flex justify-center">
						    <div class="align-center hidden-sm-and-down items"> 		         
			       			  <ul class="items">
							<ul class="d-flex">
								<v-list-item>
									<nuxt-link exact to="/" class="navLinks">Home</nuxt-link>
								</v-list-item>
								<v-list-item>
									<v-menu
      									open-on-hover
      									bottom
      									offset-y
      									transition="slide-y-transition"
    								>
		      							<template v-slot:activator="{ on, attrs }">
			        						<span
									          class="navLinks"
									          v-bind="attrs"
									          v-on="on"
									        >
									          Shop
									        </span>
		      							</template>
							      <v-list>
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/shop/shop-category/" class="dropDown">Shop Category</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/shop/product-details/" class="dropDown">Product Details</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/shop/product-checkout/" class="dropDown">Product Checkout</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/shop/confirmation/" class="dropDown">Confirmation</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/shop/shoping-cart/" class="dropDown">Shopping Cart</nuxt-link>
							          </v-list-item>
							      </v-list>
							    </v-menu></v-list-item>
								<v-list-item>
									<v-menu
      									open-on-hover
      									bottom
      									offset-y
      									transition="slide-y-transition"
    								>
		      							<template v-slot:activator="{ on, attrs }">
			        						<span
									          class="navLinks"
									          v-bind="attrs"
									          v-on="on"
									        >
									          Blog
									        </span>
		      							</template>
							      <v-list>
							          <v-list-item class="dropDown">
							          	<nuxt-link to="/blog/" class="dropDown">Blog</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link to='/blog/blog-detail/' class="dropDown">Blog Details</nuxt-link>
							          </v-list-item>
							      </v-list>
							    </v-menu>
								</v-list-item>
								<v-list-item>
									<v-menu
      									open-on-hover
      									bottom
      									offset-y
      									transition="slide-y-transition"
    								>
		      							<template v-slot:activator="{ on, attrs }">
			        						<span
									          class="navLinks"
									          v-bind="attrs"
									          v-on="on"
									        >
									          Pages
									        </span>
		      							</template>
							      <v-list>
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/auth" class="dropDown">Authorithation</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/tracking" class="dropDown">Tracking</nuxt-link>
							          </v-list-item>
							      </v-list>
							    </v-menu></v-list-item>
								<v-list-item>
									<nuxt-link exact to="/contact" class="navLinks">Contact</nuxt-link>
								</v-list-item>
							</ul>
								    </ul>
							    </div>
							</v-col>
						<v-col cols="2">
					      <div class="items buttons pa-2 hidden-sm-and-down pr-md-15 justify-center">
					      	<v-hover v-slot="{ hover }">
								<v-btn class="mr-3" icon outlined :color="hover ? 'primary' : 'gray'"><v-icon>mdi-magnify</v-icon></v-btn>
							</v-hover>
							<v-hover v-slot="{ hover }">

						    <v-badge
	        					bordered
	        					color="primary"
	       						content="3"
	        					overlap
	      					>
						        <v-btn
						          outlined
						          depressed
						          icon
						          :color="hover ? 'primary' : 'gray'"
						        >
						        <v-icon>mdi-cart</v-icon>
		                         </v-btn>
	      					</v-badge>
	      					</v-hover>
							<v-hover v-slot="{ hover }">
      							<v-btn rounded text outlined large class="ml-4 btn" :color="hover ? 'primary' : 'gray'">Buy Now</v-btn>
      						</v-hover>
						    </div>
						</v-col>							
						</v-row>
							<div>							
								<v-app-bar-nav-icon 
							    	@click="drawer = !drawer"
							        color="grey" 
							        class="hidden-md-and-up float-right"
							        >
						      	</v-app-bar-nav-icon> 										
							</div>
					</div>
		</v-app-bar>
		      	<v-navigation-drawer app v-model="drawer" color="white" width="150" right class="hidden-md-and-up">
				        <ul>
				        	<v-list-item>
				        		<nuxt-link exact class="navLinks" to="/">Home</nuxt-link>
				        	</v-list-item>
								<v-list-item>
									<v-menu
      									open-on-hover
      									left
      									offset-y
      									transition="slide-y-transition"
    								>
		      							<template v-slot:activator="{ on, attrs }">
			        						<span
									          class="navLinks"
									          v-bind="attrs"
									          v-on="on"
									        >
									          Shop
									        </span>
		      							</template>
							      <v-list>
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/shop/shop-category/" class="dropDown">Shop Category</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown" to="/shop/product-details/">
							          	<nuxt-link exact to="/shop/product-details/" class="dropDown">Product Details</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/shop/product-category/" class="dropDown">Product Checkout</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/shop/confirmation/" class="dropDown">Confirmation</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/shop/shopping-cart/" class="dropDown">Shopping Cart</nuxt-link>
							          </v-list-item>
							      </v-list>
							    </v-menu></v-list-item>
								<v-list-item>
									<v-menu
      									open-on-hover
      									left
      									offset-y
      									transition="slide-y-transition"
    								>
		      							<template v-slot:activator="{ on, attrs }">
			        						<span
									          class="navLinks"
									          v-bind="attrs"
									          v-on="on"
									        >
									          Blog
									        </span>
		      							</template>
							      <v-list>
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/blog/" class="dropDown">Blog</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/blog/blog-detail/" class="dropDown">Blog Details</nuxt-link>
							          </v-list-item>
							      </v-list>
							    </v-menu>
								</v-list-item>
								<v-list-item>
									<v-menu
      									open-on-hover
      									left
      									offset-y
      									transition="slide-y-transition"
    								>
		      							<template v-slot:activator="{ on, attrs }">
			        						<span
									          class="navLinks"
									          v-bind="attrs"
									          v-on="on"
									        >
									          Pages
									        </span>
		      							</template>
							      <v-list>
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/auth" class="dropDown">Authorization</nuxt-link>
							          </v-list-item>
							          <v-divider />
							          <v-list-item class="dropDown">
							          	<nuxt-link exact to="/tracking" class="dropDown">Tracking</nuxt-link>
							          </v-list-item>
							      </v-list>
							    </v-menu></v-list-item>
								<v-list-item>
									<nuxt-link exact to="/contact" class="navLinks">Contact</nuxt-link>
								</v-list-item>
				        </ul>
				        <v-list class="text-center">
					      	<v-hover v-slot="{ hover }">
								<v-btn class="mb-2" icon outlined :color="hover ? 'primary' : 'gray'"><v-icon>mdi-magnify</v-icon></v-btn>
							</v-hover>
							<v-hover v-slot="{ hover }">

						    <v-badge
	        					bordered
	        					color="primary"
	       						content="3"
	        					overlap
	      					>
						        <v-btn
						          outlined
						          depressed
						          icon
						          :color="hover ? 'primary' : 'gray'"
						          class='mb-2 ml-2'
						        >
						        <v-icon>mdi-cart</v-icon>
		                         </v-btn>
	      					</v-badge>
	      					</v-hover>
							<v-hover v-slot="{ hover }">
      							<v-btn rounded text outlined large class="ma-1 btn" :color="hover ? 'primary' : 'gray'">Buy Now</v-btn>
      						</v-hover>
				        </v-list>
		      	</v-navigation-drawer>	
	    </div>
</template>

<script>
	export default{
		data(){
			return{
				drawer: false,
			}
		}
	}
</script>

<style scoped>
	.navLinks{
		font-family: Ubuntu;
		font-weight: 500;
		transition: all .5s;
	}
	.navLinks:hover{
		color: blue;
		cursor: pointer;
	}
	.dropDown{
		font-family: Ubuntu;
		font-weight: 500;
		transition: all .5s;
	}
	.dropDown:hover{
		color: #ffff;
		background: blue;
	}
	.full{
 	width: 100px;
 }
 .hovered:hover{
 	color: orange;
 }
 a{
 	text-decoration: none;
 }
 a{
 	color: black;
 	font-weight: bold;
 	font-family: Ubuntu;
 }
 li{
 	list-style: none;
 	font-size: 16px;
 }
 .hovered{
 	transition: all .5s;
 }
 i:hover{
 	font-style: orange;
 }
 .auth{
 	color: #81868a;
 }
 .links{
 	margin: 0 auto;
 }
 .pos{
 	display: flex;
 	position: absolute;
 	width: 100%;
 	top: 4px;
 	/*background-color: red;*/
 }
 .center{	
 	position: absolute;
 	/*top: 33px;*/
 	max-height: 1px;
 }
 .navigation{
 	width: 100%;
 	display: flex;
 }
 .items{
 	display: flex;
 }
 .buttons{
 	background: #fff;
 }
 .app-bar{
 	background: red;
 	width: auto;
 }
 .nuxt-link-exact-active{
 	color: black;
 }
  .nuxt-link-active{
 	color: blue;
 }
</style>
