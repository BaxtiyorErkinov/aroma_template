<template>
	<div class="bg">
		<v-row>
			<v-col md="3" sm="12">
				<v-card>
					<v-card-title class="primary white--text">Browse Categories</v-card-title>
					<div class="pa-5 cont">
						<div>
						    <v-radio-group v-model="radioGroup">
							      <v-radio
							      	label="Men (3600)"
							      	class="mb-3"
							      ></v-radio>
							       <v-radio
							      	label="Women (3600)"
							      	class="mb-3"
							      ></v-radio>							     
							       <v-radio
							      	label="Accessories (3600)"
							      	class="mb-3"
							      ></v-radio>							      
							      <v-radio
							      	label="Footwear (3600)"
							      	class="mb-3"
							      ></v-radio>							     
							       <v-radio
							      	label="Bay item (3600)"
							      	class="mb-3"
							      ></v-radio>							      
							      <v-radio
							      	label="Electronics (3600)"
							      	class="mb-3"
							      ></v-radio>
							      <v-radio
							      	label="Food (3600)"
							      	class="mb-3"
							      ></v-radio>
						    </v-radio-group>
						</div>
					</div>	
				</v-card>
				<v-card class="mt-5">
					<v-card-title class="primary white--text">Product Filters</v-card-title>
					<div class="pa-5 cont">
						<div>
							<p>Brands</p>
						</div>
						<div>
						    <v-radio-group v-model="radioGroup">
							      <v-radio
							      	label="Apple (19)"
							      	class="mb-3"
							      ></v-radio>
							       <v-radio
							      	label="Asus (220)"
							      	class="mb-3"
							      ></v-radio>							     
							       <v-radio
							      	label="Artel (30)"
							      	class="mb-3"
							      ></v-radio>							      
							      <v-radio
							      	label="Micromax (60)"
							      	class="mb-3"
							      ></v-radio>							     
							       <v-radio
							      	label="Samsung (10)"
							      	class="mb-3"
							      ></v-radio>							      
						    </v-radio-group>
						</div>
					</div>	
					<v-divider />
					<div class="pa-5 cont">
						<div>
							<p>Colors</p>
						</div>
						<div>
						    <v-radio-group v-model="radioGroup">
							      <v-radio
							      	label="Black (15)"
							      	class="mb-3"
							      ></v-radio>
							       <v-radio
							      	label="Black Leather(20)"
							      	class="mb-3"
							      ></v-radio>							     
							       <v-radio
							      	label="Black with red(36)"
							      	class="mb-3"
							      ></v-radio>							      
							      <v-radio
							      	label="Gold(65)"
							      	class="mb-3"
							      ></v-radio>							     
							       <v-radio
							      	label="Spacegrey(12)"
							      	class="mb-3"
							      ></v-radio>							      
						    </v-radio-group>
						</div>
						<v-divider />
						<div class="pa-5 cont">
							<div>
								<p>Price</p>
							</div>
							<div>
								<v-slider
						        v-model="price"
						        :tick-labels="priceLabels"
						        :max="2"
						        step="1"
						        ticks="always"
						        tick-size="5"
						      ></v-slider>
							</div>
						</div>
					</div>	
				</v-card>
			</v-col>
			<v-col md="9">
				<div>
					<div class="cont mt-3">
						<v-card color="#f1f6f7" class="px-2">
							<div>
								<v-row class="pt-4">
									<v-col md="6">
										<div class="d-flex">
										<div class="item">											
										    <v-overflow-btn
										      :items="dopdown_items"
										      label="Default sorting"
										      outlined
										      class="d-flex"
										    ></v-overflow-btn>
										</div>
										<div class=item>											
										    <v-overflow-btn
										      :items="show"
										      label="Show"
										      outlined
										      class="d-flex"
										    ></v-overflow-btn>
										</div>											
										</div>
									</v-col>
									<v-col cols="6">
										<v-text-field 
											label="Search" 
											append-icon="mdi-magnify"
											outlined
										></v-text-field>
									</v-col>
								</v-row>
							</div>
						</v-card>
					</div>
				</div>
				<v-row class="mt-6">
					<v-col md="4" sm="6" cols='6'>
						<v-hover v-slot="{ hover }">
							<v-card
					      		class="mx-auto"
					      		max-width="320"
					      		flat
					    	>
					      		<v-img
					       		 :aspect-ratio="16/9"
					       		 :src="getImageUrl('product2.png')"
					       		 height="300"

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
					</v-col>
					<v-col md="4" sm="6" cols="6">
						<v-hover v-slot="{ hover }">
							<v-card
					      		class="mx-auto"
					      		max-width="320"
					      		flat
					    	>
					      		<v-img
					       		 :aspect-ratio="16/9"
					       		 :src="getImageUrl('product3.png')"
					       		 height="300"

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
					</v-col>
					<v-col md="4" sm="6" cols='6'>
						<v-hover v-slot="{ hover }">
							<v-card
					      		class="mx-auto"
					      		max-width="320"
					      		flat
					    	>
					      		<v-img
					       		 :aspect-ratio="16/9"
					       		 :src="getImageUrl('product4.png')"
					       		 height="300"

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
					</v-col>
					<v-col md="4" sm="6" cols="6">
						<v-hover v-slot="{ hover }">
							<v-card
					      		class="mx-auto"
					      		max-width="320"
					      		flat
					    	>
					      		<v-img
					       		 :aspect-ratio="16/9"
					       		 :src="getImageUrl('product5.png')"
					       		 height="300"

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
					</v-col>
					<v-col md="4" sm="6" cols='6'>
						<v-hover v-slot="{ hover }">
							<v-card
					      		class="mx-auto"
					      		max-width="320"
					      		flat
					    	>
					      		<v-img
					       		 :aspect-ratio="16/9"
					       		 :src="getImageUrl('product6.png')"
					       		 height="300"

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
					</v-col>
					<v-col md="4" sm="6" cols='6'>
						<v-hover v-slot="{ hover }">
							<v-card
					      		class="mx-auto"
					      		max-width="320"
					      		flat
					    	>
					      		<v-img
					       		 :aspect-ratio="16/9"
					       		 :src="getImageUrl('product7.png')"
					       		 height="300"

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
					</v-col>
					<v-col md="4" sm="6" cols='6'>
						<v-hover v-slot="{ hover }">
							<v-card
					      		class="mx-auto"
					      		max-width="320"
					      		flat
					    	>
					      		<v-img
					       		 :aspect-ratio="16/9"
					       		 :src="getImageUrl('product8.png')"
					       		 height="300"

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
					</v-col>
					<v-col md="4" sm="6" cols='6'>
						<v-hover v-slot="{ hover }">
							<v-card
					      		class="mx-auto"
					      		max-width="320"
					      		flat
					    	>
					      		<v-img
					       		 :aspect-ratio="16/9"
					       		 :src="getImageUrl('product3.png')"
					       		 height="300"

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
					</v-col>
					<v-col md="4" sm="6" cols="6">
						<v-hover v-slot="{ hover }">
							<v-card
					      		class="mx-auto"
					      		max-width="320"
					      		flat
					    	>
					      		<v-img
					       		 :aspect-ratio="16/9"
					       		 :src="getImageUrl('product1.png')"
					       		 height="300"

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
					</v-col>
				</v-row>
			</v-col>
		</v-row>
		<v-container>
			<shop-category-top />
		</v-container>
	</div>
</template>

<script>
	export default{
		data(){
			return{
				price: 0,
				priceLabels: ['100$', '500$', '1000$'],
				dopdown_items: ['machines', 'accessories', 'decors'],
				show: [10, 15, 25]
			}	
		},
		methods: {
			getImageUrl(img){
				return require(`@/assets/images/product/${img}`)
			}
		}
	}
</script>

<style scoped>
 .cont{
 	background: #f1f6f7;
 }
 .item{
 	width: 100%;
 	margin-right: 10px;
 }

</style>