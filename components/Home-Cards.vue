<template>
	<div>
		<v-row>
			<v-col cols="6" md="4">
				<v-hover v-slot="{ hover }">
					<v-card
			      		class="mx-auto"
			      		color="grey lighten-4"
			      		max-width="600"
			      		flat
			    	>
			      		<v-img
			       		 :aspect-ratio="16/9"
			       		 :src="getImageUrl('hero-slide1.png')"

			      		>
				       		 <v-expand-transition>
				          		<div
				            		v-if="hover"
				            		class="d-flex transition-fast-in-fast-out white darken-1 v-card--reveal text-h2 white--text align-end justify-start pa-2"
				            		style="height: 100%;"
				         		 >
				            		<v-card color="primary" dark>
				            			<v-card-title>Wirelles Headphone</v-card-title>
				            			<v-card-subtitle>Accessories Item</v-card-subtitle>
				            		</v-card>
				          		</div>
				       		 </v-expand-transition>
			      		</v-img>
			      	</v-card>
		      </v-hover>
			</v-col>
			<v-col cols="6" md="4">
		      	<v-hover v-slot="{ hover }">
					<v-card
			      		class="mx-auto"
			      		color="grey lighten-4"
			      		max-width="600"
			      		flat
			    	>
			      		<v-img
			       		 :aspect-ratio="16/9"
			       		 :src="getImageUrl('hero-slide2.png')"

			      		>
				       		 <v-expand-transition>
				          		<div
				            		v-if="hover"
				            		class="d-flex transition-fast-in-fast-out white darken-1 v-card--reveal text-h2 white--text align-end justify-start pa-2"
				            		style="height: 100%;"
				         		 >
				            		<v-card color="primary" dark>
				            			<v-card-title>Wirelles Headphone</v-card-title>
				            			<v-card-subtitle>Accessories Item</v-card-subtitle>
				            		</v-card>
				          		</div>
				       		 </v-expand-transition>
			      		</v-img>
			      	</v-card>
		      </v-hover>
			</v-col>
			<v-col cols="12" md="4">			
	      		<v-hover v-slot="{ hover }">
					<v-card
		      			class="mx-auto"
		      			color="grey lighten-4"
		      			max-width="600"
		      			flat
		    		>
			      		<v-img
			       		 :aspect-ratio="16/9"
			       		 :src="getImageUrl('hero-slide3.png')"

			      		>
				       		 <v-expand-transition>
				          		<div
				            		v-if="hover"
				            		class="d-flex transition-fast-in-fast-out white darken-1 v-card--reveal text-h2 white--text align-end justify-start pa-2"
				            		style="height: 100%;"
				         		 >
				            		<v-card color="primary" dark>
				            			<v-card-title>Wirelles Headphone</v-card-title>
				            			<v-card-subtitle>Accessories Item</v-card-subtitle>
				            		</v-card>
				          		</div>
				       		 </v-expand-transition>
			      		</v-img>
			      	</v-card>
	      		</v-hover>
			</v-col>
		</v-row>
	</div>
</template>

<script>
	export default{
		methods: {
			getImageUrl(img){
				return require(`@/assets/images/home/${img}`)
			}
		}
	}
</script>

<style scoped>
.v-card--reveal {
  align-items: center;
  bottom: 0;
  justify-content: center;
  opacity: 0.9;
  position: absolute;
  width: 100%;
}
</style>