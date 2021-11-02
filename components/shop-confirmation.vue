<template>
	<div>
		<v-row justify="center">
			<v-col cols="6">
				<v-alert
				    shaped
			        dark
				    color="info"
				    type="success"
			    >
      			Thank you. Your order has been received.
    			</v-alert>
			</v-col>
		</v-row>
		<v-row>
			<v-col md="4" sm="12" cols="12">				
				<v-card flat color="#f1f6f7" class="pa-5">
					<v-card-title>Order Info</v-card-title>
					<v-row class="my-3">
						<v-col cols="6" class="px-6 py-0">
							<p>Order number</p>
						</v-col>
						<v-col cols="6" class="py-0">: 60235</v-col>
						<v-col cols="6" class="px-6 py-0">
							<p>Date</p>
						</v-col>
						<v-col cols="6" class="py-0">: Oct 03, 2017</v-col>
						<v-col cols="6" class="px-6 py-0">
							<p>Total</p>
						</v-col>
						<v-col cols="6" class="py-0">: USD 2210</v-col>
						<v-col cols="6" class="px-6 py-0">
							<p>Payment method</p>
						</v-col>
						<v-col cols="6" class="py-0">: Check payments</v-col>
					</v-row>
				</v-card>
			</v-col>
			<v-col md="4" sm="12" cols="12">
				<v-card flat color="#f1f6f7" class="pa-5">
					<v-card-title>Billing Address</v-card-title>
					<v-row class="my-3">
						<v-col cols="6" class="px-6 py-0">
							<p>Street</p>
						</v-col>
						<v-col cols="6" class="py-0">: 56/8 panthapath</v-col>
						<v-col cols="6" class="px-6 py-0">
							<p>City</p>
						</v-col>
						<v-col cols="6" class="py-0">: Dhaka</v-col>
						<v-col cols="6" class="px-6 py-0">
							<p>Country</p>
						</v-col>
						<v-col cols="6" class="py-0">: Bangladesh</v-col>
						<v-col cols="6" class="px-6 py-0">
							<p>Postcode</p>
						</v-col>
						<v-col cols="6" class="py-0">: 1205</v-col>
					</v-row>
				</v-card>
			</v-col>
			<v-col md="4" sm="12" cols="12">
				<v-card flat color="#f1f6f7" class="pa-5">
					<v-card-title>Shipping Address</v-card-title>
					<v-row class="my-3">
						<v-col cols="6" class="px-6 py-0">
							<p>Street</p>
						</v-col>
						<v-col cols="6" class="py-0">: 56/8 panthapath</v-col>
						<v-col cols="6" class="px-6 py-0">
							<p>City</p>
						</v-col>
						<v-col cols="6" class="py-0">: Dhaka</v-col>
						<v-col cols="6" class="px-6 py-0">
							<p>Country</p>
						</v-col>
						<v-col cols="6" class="py-0">: Bangladesh</v-col>
						<v-col cols="6" class="px-6 py-0">
							<p>Postcode</p>
						</v-col>
						<v-col cols="6" class="py-0">: 1205</v-col>
					</v-row>
				</v-card>
			</v-col>
		</v-row>
		<v-card flat color="#f1f6f7" class="pa-5 mt-7 mb-7">
			<v-card-title class="mb-3 text-h4 font-weight-medium">Order Details</v-card-title>
			<v-row align="center">
				<v-col cols="12" class="py-1">
					<v-divider />
				</v-col>
				<v-col cols="5" md="6" sm="6" class="px-6 py-1">
					<div class="text-h6 font-weight-black">Product</div>
				</v-col>
				<v-col cols="4" md="2" sm="2" class="font-weight-black py-1">Quantity</v-col>
				<v-col cols="3" md="4" sm="4" class="font-weight-black py-1">Total</v-col>
				<v-col cols="12" class="py-1">
					<v-divider />
				</v-col>
				<v-col cols="5" md="6" sm="6" class="px-6">
					<div class="grey--text">Pixelstore fresh Blackberry</div>
				</v-col>
				<v-col cols="3" md="2" sm="2" class="font-weight-medium">X 02</v-col>
				<v-col cols="4" class="grey--text">$720.00</v-col>
				<v-col cols="5" md="6" sm="6" class="px-6">
					<div class="grey--text">Pixelstore fresh Blackberry</div>
				</v-col>
				<v-col cols="3" md="2" sm="2" class="font-weight-medium">X 02</v-col>
				<v-col cols="4" class="grey--text">$720.00</v-col>
				<v-col cols="5" md="6" sm="6" class="px-6">
					<div class="grey--text">Pixelstore fresh Blackberry</div>
				</v-col>
				<v-col cols="3" md="2" sm="2" class="font-weight-medium">X 02</v-col>
				<v-col cols="4" class="grey--text">$720.00</v-col>
				<v-col cols="8" class="px-6">
					<div class="font-weight-medium">SUBTOTAL</div>
				</v-col>
				<v-col cols="4" class="grey--text">$2160.00</v-col>
				<v-col cols="8" class="px-6">
					<div class="font-weight-medium">SHIPPING</div>
				</v-col>
				<v-col cols="4" class="grey--text">Flat rate: $50.00</v-col>
				<v-col cols="12">
					<v-divider />
				</v-col>
				<v-col cols="8" class="px-6">
					<div class="font-weight-medium">TOTAL</div>
				</v-col>
				<v-col cols="4">$2210.00</v-col>
			</v-row>
		</v-card>
	</div>
</template>