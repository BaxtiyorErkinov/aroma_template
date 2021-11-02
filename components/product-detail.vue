<template>
	<div class="mt-5 mb-5">
		<v-row>
			<v-col md="6">
				<v-img :src="getImg('product1.png')" />
			</v-col>
			<v-col md="6">
				<v-card class="pa-10" flat>
					<v-card-title class="text-h4">Faded SkyBlu Denim Jeans</v-card-title>
					<v-card-subtitle class="primary--text text-h4 pa-4 font-weight-medium">$149.99</v-card-subtitle>
					<div class="pa-5">
						<p>Category : <span class="grey--text">Household</span></p>
						<p>Availibility : <span class="grey--text">In Stock</span></p>
					</div>
					<div class="pa-3">
						<p>Mill Oil is an innovative oil filled radiator with the most modern technology. If you are looking for something that can make your interior look awesome, and at the same time give you the pleasant warm feeling during the winter.</p>
					</div>
					<div class='pa-2'>
						<v-row class="align-content-center">
							<v-col cols="12" md='3'>
								<p class="mt-2">Quantity :</p>
							</v-col>
							<v-col cols="6" md='2'>
								<v-text-field type="number" outlined dense small value="1"/>
							</v-col>
							<v-col cols="6" md="2">
								<v-btn color="primary">Add to Cart</v-btn>
							</v-col>
						</v-row>
					</div>
					<div class="pa-3">
						<div>
							<v-btn color="primary"><v-icon>mdi-diamond-stone</v-icon></v-btn>
							<v-btn color="primary"><v-icon>mdi-heart-outline</v-icon></v-btn>
						</div>
					</div>
				</v-card>
			</v-col>
		</v-row>
		<v-card color="basil" class="mt-4">
		    <v-tabs
		      v-model="tab"
		      background-color="#f1f6f7"
		 	  grow
		      color="deep-purple accent-4"
		    >
		      <v-tab>
		        Description
		      </v-tab>
		      <v-tab>
		        Specification
		      </v-tab>
		      <v-tab>
		        Comments
		      </v-tab>
		      <v-tab>
		        Reviews
		      </v-tab>
		    </v-tabs>

		    <v-tabs-items v-model="tab">
		      <v-tab-item>
		        <v-card
		          color="basil"
		          flat
		          class="pa-5"
		        >
		          <div class="mt-2">
		          	<p class='grey--text'>Beryl Cook is one of Britain’s most talented and amusing artists .Beryl’s pictures feature women of all shapes and sizes enjoying themselves .Born between the two world wars, Beryl Cook eventually left Kendrick School in Reading at the age of 15, where she went to secretarial school and then into an insurance office. After moving to London and then Hampton, she eventually married her next door neighbour from Reading, John Cook. He was an officer in the Merchant Navy and after he left the sea in 1956, they bought a pub for a year before John took a job in Southern Rhodesia with a motor company. Beryl bought their young son a box of watercolours, and when showing him how to use it, she decided that she herself quite enjoyed painting. John subsequently bought her a child’s painting set for her birthday and it was with this that she produced her first significant work, a half-length portrait of a dark-skinned lady with a vacant expression and large drooping breasts. It was aptly named ‘Hangover’ by Beryl’s husband and</p>
		          </div>
		          <div class='mt-3'>
		          	<p class='grey--text'>It is often frustrating to attempt to plan meals that are designed for one. Despite this fact, we are seeing more and more recipe books and Internet websites that are dedicated to the act of cooking for one. Divorce and the death of spouses or grown children leaving for college are all reasons that someone accustomed to cooking for more than one would suddenly need to learn how to adjust all the cooking practices utilized before into a streamlined plan of cooking that is more efficient for one person creating less</p>
		          </div>
		        </v-card>
		      </v-tab-item>
		      <v-tab-item>
		        <v-card
		          color="basil"
		          flat
		          class="pa-5"
		        >
		          <v-row>
		          	<v-col cols='12'>
		          		<v-row class="ml-3 grey--text font">
		          			<v-col cols='6'><p>Width</p></v-col>
		          			<v-col cols='6'><p>128mm</p></v-col>
		          		</v-row>
		          	<v-divider />
		          	</v-col>
		          	<v-col cols='12'>
		          		<v-row class="ml-3 grey--text font">
		          			<v-col cols='6'><p>Height</p></v-col>
		          			<v-col cols='6'><p>508mm</p></v-col>
		          		</v-row>
		          	<v-divider />
		          	</v-col>
		          	<v-col cols='12'>
		          		<v-row class="ml-3 grey--text font">
		          			<v-col cols='6'><p>Depth</p></v-col>
		          			<v-col cols='6'><p>85mm</p></v-col>
		          		</v-row>
		          	<v-divider />
		          	</v-col>
		          	<v-col cols='12'>
		          		<v-row class="ml-3 grey--text font">
		          			<v-col cols='6'><p>Weight</p></v-col>
		          			<v-col cols='6'><p>52gm</p></v-col>
		          		</v-row>
		          	<v-divider />
		          	</v-col>
		          	<v-col cols='12'>
		          		<v-row class="ml-3 grey--text font">
		          			<v-col cols='6'><p>Quality Checking</p></v-col>
		          			<v-col cols='6'><p>Yes</p></v-col>
		          		</v-row>
		          	<v-divider />
		          	</v-col>
		          	<v-col cols='12'>
		          		<v-row class="ml-3 grey--text font">
		          			<v-col cols='6'><p>Freshness Duration</p></v-col>
		          			<v-col cols='6'><p>03 Days</p></v-col>
		          		</v-row>
		          	<v-divider />
		          	</v-col>
		          	<v-col cols='12'>
		          		<v-row class="ml-3 grey--text font">
		          			<v-col cols='6'><p>When packeting</p></v-col>
		          			<v-col cols='6'><p>Without touch of hand</p></v-col>
		          		</v-row>
		          	<v-divider />
		          	</v-col>
		          	<v-col cols='12'>
		          		<v-row class="ml-3 grey--text font">
		          			<v-col cols='6'><p>Each Box contains</p></v-col>
		          			<v-col cols='6'><p>60pcs</p></v-col>
		          		</v-row>
		          	</v-col>
		          </v-row>
		        </v-card>
		      </v-tab-item>
		      <v-tab-item>
		        <v-card
		          color="basil"
		          flat
		        >
		          <v-row>
		          	<v-col cols="12" md="6" sm="12"> 
		          		<v-card class="pa-3" tile flat>
		          			<v-row class="align-center">
		          				<v-col cols='3' md='2' sm="2">
		          					<v-avatar size="80">
		          						<img :src="getImg('review-1.png')" />
		          					</v-avatar>
		          				</v-col>
		          				<v-col cols='5'>
		          					<div>
		          						<span class="font-weight-medium">Blake Ruiz</span>
		          					</div>
		          						<span class="grey--text">12th Feb, 2018 at 05:56 pm</span>
		          				</v-col>
		          				<v-col cols="5" class=" d-flex justify-end">
		          					<v-btn rounded small outlined text>Reply</v-btn>
		          				</v-col>
		          				<v-col cols="12" class="pa-5">
		          					<p class="grey--text">
		          						Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
		          					</p>
		          				</v-col>
		          			</v-row>
		          		</v-card>
		          		<v-card class="pa-10" tile flat>
		          			<v-row class="align-center">
		          				<v-col cols='4' md='2' sm="2">
		          					<v-avatar size="80" >
		          						<img :src="getImg('review-2.png')" />
		          					</v-avatar>
		          				</v-col>
		          				<v-col cols='5'>
		          					<div>
		          						<span class="font-weight-medium">Blake Ruiz</span>
		          					</div>
		          						<span class="grey--text">12th Feb, 2018 at 05:56 pm</span>
		          				</v-col>
		          				<v-col cols="5" class=" d-flex justify-end">
		          					<v-btn rounded small outlined text>Reply</v-btn>
		          				</v-col>
		          				<v-col cols="12" class="pa-5">
		          					<p class="grey--text">
		          						Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
		          					</p>
		          				</v-col>
		          			</v-row>
		          		</v-card>
		          		<v-card class="pa-3" tile flat>
		          			<v-row class="align-center">
		          				<v-col cols='3' md='2' sm="2">
		          					<v-avatar size="80">
		          						<img :src="getImg('review-3.png')" />
		          					</v-avatar>
		          				</v-col>
		          				<v-col cols='5'>
		          					<div>
		          						<span class="font-weight-medium">Blake Ruiz</span>
		          					</div>
		          						<span class="grey--text">12th Feb, 2018 at 05:56 pm</span>
		          				</v-col>
		          				<v-col cols="5" class=" d-flex justify-end">
		          					<v-btn rounded small outlined text>Reply</v-btn>
		          				</v-col>
		          				<v-col cols="12" class="pa-5">
		          					<p class="grey--text">
		          						Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
		          					</p>
		          				</v-col>
		          			</v-row>
		          		</v-card>
		          	</v-col>
		          	<v-col cols="12" md="6" sm="12">
		          		<v-card tile flat class="pa-5">
		          			<v-card-title class="mb-5 font-weight-regular">Post a Comment</v-card-title>
		          			<div>
		          				<v-row class="justify-center">
		          					<v-form>
		          						<v-col cols="12">
		          							<v-text-field outlined dense label="Your Full Name" height="20"/>
		          						</v-col>
		          						<v-col cols='12'>
		          							<v-text-field outlined dense label="Your Email Address"/>
		          						</v-col>
		          						<v-col cols='12'>
		          							<v-text-field outlined dense label="Your Phone Number"/>
		          						</v-col>
		          						<v-col cols='12'>
		          							<v-textarea 
		          							outlined 
		          							dense           
		          							auto-grow
								    		outlined
								          	rows="3"
								          	row-height="25"
								          	shaped 
								          	label="Message ..."/>
		          						</v-col>
		          						<v-col cols='12' class="d-flex justify-end">
		          							<v-btn color="primary">Submit Now</v-btn>
		          						</v-col>
		          					</v-form>
		          				</v-row>
		          			</div>
		          		</v-card>
		          	</v-col>
		          </v-row>
		        </v-card>
		      </v-tab-item>
		      <v-tab-item>
		        <v-card
		          color="basil"
		          flat
		          class="pa-5"
		        >
		         <v-row>
		         	<v-col cols="12" md="7" sm="12">
		         		<v-row>
		         			<v-col cols="12" md="6" sm="6">
		         				<v-card color="#f1f6f7" class="pa-5" text-center flat>
		         					<div class="text-center">
		         						<p class="text-h4 font-weight-medium">Overall</p>
		         					</div>
		         					<div class="text-center">
		         						<p class="primary--text text-h3 font-weight-bold">4.0</p>
		         					</div>
		         					<div class="text-center">
		         						<p>(03 Reviews)</p>
		         					</div>
		         				</v-card>
		         			</v-col>
		         			<v-col cols="12" md="6" sm='6'>
		         				<v-card flat class="px-7">
		         					<div class="text-start">
		         						<p class="font-weight-medium text-h5">Based on 3 Reviews</p>
		         						<div class='pa-1'>
			         						<div class="d-flex">		         								
			         							<span class="font mt-1">5 star</span>
			         							<v-rating
											      value="5"
											      length="5"
											      background-color="warning lighten-3"
											      color="yellow"
											      size="18"
											    />
			         						</div>
			         						<div class="d-flex">		         								
			         							<span class="font mt-1">4 star</span>
			         							<v-rating
											      value="5"
											      length="5"
											      background-color="warning lighten-3"
											      color="yellow"
											      size="18"
											    />
			         						</div>
			         						<div class="d-flex">		         								
			         							<span class="font mt-1">3 star</span>
			         							<v-rating
											      value="5"
											      length="5"
											      background-color="warning lighten-3"
											      color="yellow"
											      size="18"
											    />
			         						</div>
			         						<div class="d-flex">		         								
			         							<span class="font mt-1">2 star</span>
			         							<v-rating
											      value="5"
											      length="5"
											      background-color="warning lighten-3"
											      color="yellow"
											      size="18"
											    />
			         						</div> 
			         						<div class="d-flex">		         								
			         							<span class="font mt-1">1 star</span>
			         							<v-rating
											      value="5"
											      length="5"
											      background-color="warning lighten-3"
											      color="yellow"
											      size="18"
											    />
			         						</div>
		         						</div>
		         					</div>
		         				</v-card>
		         			</v-col>
		         			<v-col cols='12'>
		         				<v-card class="pa-3" tile flat>
				          			<v-row class="align-center">
				          				<v-col cols='4' md='2' sm="2">
				          					<v-avatar size="80">
				          						<img :src="getImg('review-3.png')" />
				          					</v-avatar>
				          				</v-col>
				          				<v-col cols='5'>
				          					<div>
				          						<span class="font-weight-medium">Blake Ruiz</span>
				          					</div>
				          						<span>
				          							<v-rating
													      value="5"
													      length="5"
													      background-color="warning lighten-3"
													      color="yellow"
													      size="18"
													    />
				          						</span>
				          				</v-col>
				          				<v-col cols="5" class=" d-flex justify-end">
				          					<v-btn rounded small outlined text>Reply</v-btn>
				          				</v-col>
				          				<v-col cols="12" class="pa-5">
				          					<p class="grey--text">
				          						Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
				          					</p>
				          				</v-col>
				          			</v-row>
		          				</v-card>
		         			</v-col>
		         			<v-col cols='12'>
		         				<v-card class="pa-3" tile flat>
				          			<v-row class="align-center">
				          				<v-col cols='4' md='2' sm="2">
				          					<v-avatar size="80">
				          						<img :src="getImg('review-1.png')" />
				          					</v-avatar>
				          				</v-col>
				          				<v-col cols='5'>
				          					<div>
				          						<span class="font-weight-medium">Blake Ruiz</span>
				          					</div>
				          						<span>
				          							<v-rating
													      value="5"
													      length="5"
													      background-color="warning lighten-3"
													      color="yellow"
													      size="18"
													    />
				          						</span>
				          				</v-col>
				          				<v-col cols="5" class=" d-flex justify-end">
				          					<v-btn rounded small outlined text>Reply</v-btn>
				          				</v-col>
				          				<v-col cols="12" class="pa-5">
				          					<p class="grey--text">
				          						Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
				          					</p>
				          				</v-col>
				          			</v-row>
		          				</v-card>
		         			</v-col>
		         			<v-col cols='12'>
		         				<v-card class="pa-3" tile flat>
				          			<v-row class="align-center">
				          				<v-col cols='4' md='2' sm="2">
				          					<v-avatar size="80">
				          						<img :src="getImg('review-2.png')" />
				          					</v-avatar>
				          				</v-col>
				          				<v-col cols='5'>
				          					<div>
				          						<span class="font-weight-medium">Blake Ruiz</span>
				          					</div>
				          						<span>
				          							<v-rating
													      value="5"
													      length="5"
													      background-color="warning lighten-3"
													      color="yellow"
													      size="18"
													    />
				          						</span>
				          				</v-col>
				          				<v-col cols="5" class=" d-flex justify-end">
				          					<v-btn rounded small outlined text>Reply</v-btn>
				          				</v-col>
				          				<v-col cols="12" class="pa-5">
				          					<p class="grey--text">
				          						Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
				          					</p>
				          				</v-col>
				          			</v-row>
		          				</v-card>
		         			</v-col>
		         		</v-row>
		         	</v-col>
		         	<v-col cols="12" md="5" sm='12'>
		         		<v-card tile flat class="">
		          			<v-card-title class="font-weight-medium">Add a Review</v-card-title>
		          			<div class="d-flex mb-5 px-5">		         								
			         			<span class="font mt-1">Your Rating: </span>
			         				<v-rating
									    value="5"
										length="5"
							   	        background-color="warning lighten-3"
							    	    color="yellow"
										size="18"
									    />
			       			</div>
		          			<div>
		          				<v-row class="justify-center">
		          					<v-form>
		          						<v-col cols="12">
		          							<v-text-field outlined dense label="Your Full Name" height="20"/>
		          						</v-col>
		          						<v-col cols='12'>
		          							<v-text-field outlined dense label="Your Email Address"/>
		          						</v-col>
		          						<v-col cols='12'>
		          							<v-text-field outlined dense label="Your Phone Number"/>
		          						</v-col>
		          						<v-col cols='12'>
		          							<v-textarea 
		          							outlined 
		          							dense           
		          							auto-grow
								    		outlined
								          	rows="3"
								          	row-height="25"
								          	shaped 
								          	label="Message ..."/>
		          						</v-col>
		          						<v-col cols='12' class="d-flex justify-end">
		          							<v-btn color="primary" rounded>Submit Now</v-btn>
		          						</v-col>
		          					</v-form>
		          				</v-row>
		          			</div>
		          		</v-card>
		         	</v-col>
		         </v-row>
		        </v-card>
		      </v-tab-item>
		    </v-tabs-items>
 	 </v-card>
	</div>
</template>

<script>
	export default{
		data() {
			return{
				tab: null,
				rating: 5,
			}
		},
		methods: {
			getImg(img){
				return require(`~/assets/images/product/${img}`)
			}
		}
	}
</script>

<style scoped>
	.font{
		font-family: Ubuntu;
	}
</style>