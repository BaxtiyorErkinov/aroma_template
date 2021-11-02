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
		          Shopping Cart
		        </h1>
		        <p class="grey--text">
		        	Home - Shopping Cart
		        </p>	
		      </v-col>
		    </v-row>
		</v-parallax>
		<v-container>
			<shop-cart />
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