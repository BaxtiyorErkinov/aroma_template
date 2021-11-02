<template>
	<div class="bg">
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
	          Shop Category
	        </h1>
	        <p class="grey--text">
	        	Home - Shop Category
	        </p>	
	      </v-col>
	    </v-row>
	  </v-parallax>
	  <v-container color="#f8f9fa">
	  	<shop-category />
	  </v-container>
	  <v-container>
      	<Home-form />
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

</style>