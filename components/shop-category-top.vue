<template>
	<div>
		<div class="mb-10 mt-5">
			<h5 class="home-title">Popular Item in the market</h5>
			<h2 class='home-subtitle'>Top <span class="subtitle-item">Product</span></h2>
		</div>
		<v-row>
			<v-col md="3" sm="6" cols="12">
				<v-card tile flat class="pa-3" outlined>
					<v-row>				
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-1.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-2.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-3.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
					</v-row>
				</v-card>
			</v-col>
			<v-col md="3" sm="6" cols='12'>
				<v-card tile flat class="pa-3" outlined>
					<v-row>				
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-4.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-5.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-6.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
					</v-row>
				</v-card>
			</v-col>
			<v-col md="3" sm="6" cols='12'>
				<v-card tile flat class="pa-3" outlined>
					<v-row>				
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-7.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-6.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-4.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
					</v-row>
				</v-card>
			</v-col>
			<v-col md="3" sm="6" cols='12'>
				<v-card tile flat class="pa-3" outlined>
					<v-row>				
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-1.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-2.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
						<v-col cols='12'>
							<v-container>							
								<div>
									<v-row>
										<v-col cols="4">
											<v-img :src="getImageUrl('product-sm-3.png')" height="70" width="100"></v-img>
										</v-col>
										<v-col cols="8">
											<h4>Gray Coffe Cup</h4>
											<p class="mt-3">$170.00</p>
										</v-col>
									</v-row>
								</div>
							</v-container>
						</v-col>
					</v-row>
				</v-card>
			</v-col>
		</v-row>

	</div>
</template>

<script>
	export default{
		methods: {
			getImageUrl(img){
				return require(`@/assets/images/product/${img}`)
			}
		}
	}
</script>

<style scoped>
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