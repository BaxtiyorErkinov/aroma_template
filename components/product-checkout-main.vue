<template>
	<div>
		<v-row>
			<v-col cols="12">
				<v-card flat color="#f8f9fa" class="pa-4">
					<div>
						<span>Returning Customer?<a href="#" class="ml-3">Click here to login</a></span>
					</div>
				</v-card>
			</v-col>
			<v-col cols="12">
				<v-card flat>
					<div>
						<p>If you have shopped with us before, please enter your details in the boxes below. If you are a new customer, please proceed to the Billing & Shipping section.</p>
					</div>
					<v-form>
						<v-row>
							<v-col cols="4">
								<v-text-field label="Username or Email*"/>
							</v-col>
							<v-col cols="4">
								<v-text-field label="Password*"/>
							</v-col>
							<v-col cols="12">
								<v-row class="align-center">
									<v-col cols="3" md="1" sm="2">								
										<v-btn rounded color="primary" depressed>login</v-btn>
									</v-col>
									<v-col cols="2">
										<v-checkbox label="Remember me"/>
									</v-col>
								</v-row>	
							</v-col>
							<v-col cols="12">
								<v-card flat color="#f8f9fa" class="pa-4">
									<div>
										<span>Have a coupon?<a href="#" class="ml-3"> Click here to enter your code</a></span>
									</div>
								</v-card>
							</v-col>
							<v-col cols="8">
								<v-text-field label="Enter cupon code"/>
							</v-col>
							<v-col cols="8">
								<v-btn color="primary" depressed rounded>Apply Coupon</v-btn>
							</v-col>	
						</v-row>
				    </v-form>
				</v-card>
			</v-col>
		</v-row>
		<v-row>
			<v-col cols="12" md="8">
				<v-card flat>
					<v-card-title class="font-weight-black">Billing Details</v-card-title>
					<v-divider />
					<v-row class="mt-2">
						<v-col cols="6">
							<v-text-field outlined dense/>
						</v-col>
						<v-col cols="6">
							<v-text-field outlined dense/>
							
						</v-col>
						<v-col cols="12">
							<v-text-field outlined dense label="Company Name"/>
							
						</v-col>
						<v-col cols='6'>
							<v-text-field outlined dense/>
							
						</v-col>
						<v-col cols="6">
							<v-text-field outlined dense/>
							
						</v-col>
						<v-col cols="12">
							<v-select outlined dense label="Country" :items="countrys"/>
							
						</v-col>
						<v-col cols="12">
							<v-text-field outlined dense/>
							
						</v-col>
						<v-col cols="12">
							<v-text-field outlined dense/>
							
						</v-col>
						<v-col cols="12">
							<v-text-field outlined dense/>
							
						</v-col>
						<v-col cols="12">
							<v-select outlined dense label="District" :items="countrys"/>
							
						</v-col>
						<v-col cols="12">
							<v-text-field outlined dense label="PostCode/ZIP"/>
						</v-col>
					</v-row>
					<div>
						<v-checkbox label="Create an account?"/>
					</div>
					<div class="mb-2">
						<h2>Shipping Details</h2>
					</div>
					<v-divider />
					<div>
						<v-checkbox label="Ship to a different address?"/>
					</div>
					<div>
						<v-textarea label="Order Notes" outlined/>
					</div>
				</v-card>
			</v-col>
			<v-col cols="12" md="4">
				<v-card color="#f1f6f7" class="pa-3 px-5" flat>
					<v-card-title>Your Order</v-card-title>
					<v-divider />
					<v-row class="mt-2">
						<v-col cols="6"><p class="text">Product</p></v-col>
						<v-col cols="6" class="text-right text"><p>Total</p></v-col>
						<v-col cols="6"><p class="text grey--text">Fresh Blackberry</p></v-col>
						<v-col cols="3"><p class="text">x 02</p></v-col>
						<v-col cols="3"><p class="text grey--text">$720.00</p></v-col>
						<v-col cols="6"><p class="text grey--text">Fresh Tomatoes</p></v-col>
						<v-col cols="3"><p class='text'>x 02</p></v-col>
						<v-col cols="3"><p class="text grey--text">$720.00</p></v-col>
						<v-col cols="6"><p class="text">Fresh Brocoli</p></v-col>
						<v-col cols="3"><p class="text">x 02</p></v-col>
						<v-col cols="3"><p class='text grey--text'>$720.00</p></v-col>
						<v-col cols="6"><p class="text">SUBTOTAL</p></v-col>
						<v-col cols="6" class="text-right text grey--text"><p>$2160.00</p></v-col>
						<v-col cols="6"><p class='text'>SHIPPING</p></v-col>
						<v-col cols="6" class="text-right text"><p class="grey--text">Flat Rate: $50.00</p></v-col>
						<v-col cols="6"><p class="text">TOTAL</p></v-col>
						<v-col cols="6" class="text-right text"><p>$2210.00</p></v-col>
						<v-radio-group v-model="radioGroup">
							<v-col cols='12'>
	      							<v-radio
	        							color="red"
	        							label="Check Payments"
							     	 >
							      </v-radio>
							    <v-card flat>
							    	<v-container class="grey--text">
							    		<span class="text-1">Please send a check to Store Name, Store Street, Store Town, Store State / County, Store Postcode.</span>
							    	</v-container>
							    </v-card>
							</v-col>
							<v-col cols='12'>
	      							<v-radio
	        							color="red"
	        							label="Paypal"
							     	 >
							      </v-radio>
							    <v-card flat>
							    	<v-container class="grey--text">
							    		<span class="text-1">Pay via PayPal; you can pay with your credit card if you don’t have a PayPal account.</span>
							    	</v-container>
							    </v-card>
							</v-col>
						</v-radio-group>
						<v-col cols='12'>
							<v-checkbox label="Accept the terms & conditions*"/>
						</v-col>
						<v-col cols="12" class="text-center mb-2">
							<v-btn depressed rounded large color="primary">Proceed to Paypal</v-btn>
						</v-col>
					</v-row>
				</v-card>
			</v-col>
		</v-row>
	</div>
</template>
<script>
	export default{
		data (){
			return{
				countrys: ['Uzbekistan', 'USA', 'Russia'],
				radioGroup: 1,
			}
		}
	}
</script>

<style scoped>
	.text{
		font-size: 14px;
	}
	.text-1{
		font-size: 12px;
	}
</style>