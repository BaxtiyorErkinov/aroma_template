<template>
	<div>
		<v-card flat class="mb-5 mt-5 pa-5">
			<v-row>
				<v-col cols="9" md="5" sm="5">
					<div class="font-weight-black">Product</div>
				</v-col>
				<v-col cols="3" md="2" sm="2">
					<div class="font-weight-medium">Price</div>
				</v-col>
				<v-col cols="9" md="3" sm="3">
					<div class="font-weight-medium">Quantity</div>
				</v-col>
				<v-col cols="3" md="2" sm="2">
					<div class="font-weight-medium">Total</div>
				</v-col>
				<v-col cols="12">
					<v-divider />
				</v-col>
				</v-row>
				<v-row v-for="product in products" :key="product.id" class="align-center">					
					<v-col cols="12" md="5" sm="5">
						<v-row align="center">
							<v-col cols="5">
								<v-img :src="require(`@/assets/images/cart/${product.img}`)" width="150" height="80"/>
							</v-col>
							<v-col cols="6">
								<p class="font grey--text">{{product.title}}</p>
							</v-col>
						</v-row>
					</v-col>
					<v-col cols="4" md="2" sm="2">
						<div class="font-weight-medium">{{product.price}}</div>
					</v-col>
					<v-col cols="4" md="3" sm="3">
						<v-row>
							<v-col cols="6">						
								<div class="font-weight-medium">
									<v-text-field  type="number" dense :value="product.quantity"/>
								</div>
							</v-col>
						</v-row>
					</v-col>
					<v-col cols="4" md="2" sm="2">
						<div class="font-weight-medium">{{product.total}}</div>
					</v-col>
					<v-col cols="12">
						<v-divider />
					</v-col>
				</v-row>
				<v-row>
					<v-col cols="6" md="6" sm="5">
						<v-btn depressed outlined rounded color="grey"><span class="black--text footer-text">Update Cart</span></v-btn>
					</v-col>
					<v-col cols="6" md="2" sm="2">
						<v-text-field rounded outlined dense color="grey" placeholder="Coupon Code"/>
					</v-col>
					<v-col cols="5" md="2" sm="2">
						<v-btn rounded depressed color="primary">Apply Shop</v-btn>
					</v-col>
					<v-col cols="5" md="2" sm="1">
						<v-btn rounded depressed outlined color="grey" class="ml-sm-2"><span class="black--text footer-text">Have a Coupon?</span></v-btn>
					</v-col>
					<v-col cols='12' class="pt-0">
						<v-divider />
					</v-col>
					<v-col cols="10" md='6'>
						<div class="text-h6">Subtotal:<span class="ml-3">$2160.00</span></div>
					</v-col>
					<v-col cols='12' md='3' class="text-center">
						<v-btn rounded depressed>Continue Shopping</v-btn>
					</v-col>
					<v-col cols="12" md="3" class="text-center">
						<v-btn rounded depressed color='primary'>Proceed To Checkout</v-btn>
					</v-col>
				</v-row>				
		</v-card>
	</div>
</template>

<script>
	export default {
		data(){
			return{
				products: [
					{
						id: 1,
						title: 'Minimalistic shop for multipurpose use',
						price: '$360.00',
						quantity: '1',
						total: '$720.00',
						img: 'cart1.png'
					},
					{
						id: 2,
						title: 'Minimalistic shop for multipurpose use',
						price: '$360.00',
						quantity: '1',
						total: '$720.00',
						img: 'cart2.png'
					},
					{
						id: 3,
						title: 'Minimalistic shop for multipurpose use',
						price: '$360.00',
						quantity: '1',
						total: '$720.00',
						img: 'cart3.png'
					}
				]
			}
		}
	}
</script>
<style scoped>
	.font{
		font-size: 12px;
		font-family: Ubuntu;
	}
	.footer-text{
		font-family: Ubuntu;
	}
</style>