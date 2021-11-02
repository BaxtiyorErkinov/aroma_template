<template>
	<div>		    	
	  <v-parallax
	    dark
	    :src="getImageUrl('parallax-bg.png')"
	    top
	    class="pa-0 px-16"
	  >
	    <v-row
	      align="center"
	      justify="center"
	    >
	      <v-col
	        class="d-flex"
	        cols="12"
	      >
	      <div class="text-center">      	
		        <h2 class="text-h2 font-weight-regular mb-4 black--text hidden-md-and-down">
		          Up To 50% Off
		        </h2>
		        <h3 class="black--text">Winter Sale</h3>
		        <p class="black--text">Him she'd let them sixth saw light</p>
		        <v-btn rounded x-large class="primary">Shop Now</v-btn>
	      </div>
	      </v-col>
	    </v-row>
	  </v-parallax>
	  <v-container>
	  	<NewsCard />
	  </v-container>
	</div>
</template>

<script>
	export default{
		methods:{
			getImageUrl(img){
				return require(`~/assets/images/home/${img}`)
			}
		}
	}
</script>

<style scoped>
	.btn{
		z-index: 2000;
		background-color: blue;
	}
</style>