<template>
	<div>
		<v-parallax
		    dark
		    :src="getImageUrl('bg.jpg')"
		    top
		    class="pa-0 px-0 ll"
		  >
		    <v-row
		      align="center"
		      justify="center"
		    >
		      <v-col
		        class="text-center"
		        cols="12"
		      >
		        <h1 class="text-h3 font-weight-bold mb-4 black--text">
		          Order Tracking
		        </h1>
		        <p class="grey--text">
		        	Home - Order Tracking
		        </p>	
		      </v-col>
		    </v-row>
		</v-parallax>
		<v-container class="mb-5">
			<v-row>
				<v-col cols="12">
					<v-card flat>
						<div class="pr-md-15">
							<p class="subtitle">
								To track your order please enter your Order ID in the box below and press the "Track" button. This was given to you on your receipt and in the confirmation email you should have received.
							</p>
						</div>
						<v-row class="mt-2">
							<v-col cols="12" md="7" sm="7" class="py-0">
								<v-text-field solo dense flat outlined placeholder="Order ID"/>
							</v-col>
							<v-col cols="12" md="7" sm="7" class="py-0">
								<v-text-field solo dense flat outlined placeholder="Order ID"/>
							</v-col>
							<v-col cols="7">
								<v-btn color="primary" rounded large>Track Order</v-btn>
							</v-col>
						</v-row>
					</v-card>
				</v-col>
			</v-row>
		</v-container>
	</div>
</template>

<script>
	export default{
		methods: {
			getImageUrl (img){
				return require(`~/assets/images/blog/${img}`)
			}
		}
	}
</script>

<style scoped>
	.subtitle{
		font-size: 14px;
		font-family: Ubuntu;
		color: rgba(0,0,0,0.6);
	}
</style>