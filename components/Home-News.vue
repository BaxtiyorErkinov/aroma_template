<template>
	<div>
		<div class="mb-10 mt-5">
			<h5 class="home-title">Popular Item in the market</h5>
			<h2 class='home-subtitle'>Latest <span class="subtitle-item">News</span></h2>
		</div>
		<v-row>
			<v-col md='4' cols='12' sm="4">
				<v-hover v-slot="{ hover }">
					<v-card flat>
						<v-img :src="getImg('blog1.png')"/>
						<div class="d-flex mt-3">
							<div class="d-flex">
								<p class="grey--text">By Admin</p>
							</div>
							<div class="d-flex ml-3">
								<v-btn text x-small class="d-flex" color="grey">
									<v-icon class="mr-1">mdi-chat-processing-outline</v-icon>
									<span>comments</span>
								</v-btn>
							</div>
						</div>
						<div>
							<h4 class="font-weight-medium" :class="hover ? 'primary--text' : ''">The Richland Center Shooping News and weekly shooper</h4>
						</div>
						<div class="mt-2">
							<p class="grey--text">Let one fifth i bring fly to divided face for bearing divide unto seed. Winged divided light Forth.</p>
						</div>
						<div>
							<v-btn text small class="py-5" :class="hover ? 'primary' : ''">
								<span>Read More</span>
								<v-icon :class="hover ? 'ml-2' : ''">mdi-arrow-right</v-icon>
							</v-btn>
						</div>
					</v-card>
				</v-hover>
			</v-col>
			<v-col md="4" sm="4" cols="12">
				<v-hover v-slot="{ hover }">
					<v-card flat>
						<v-img :src="getImg('blog2.png')"/>
						<div class="d-flex mt-3">
							<div class="d-flex">
								<p class="grey--text">By Admin</p>
							</div>
							<div class="d-flex ml-3">
								<v-btn text x-small class="d-flex" color="grey">
									<v-icon class="mr-1">mdi-chat-processing-outline</v-icon>
									<span>comments</span>
								</v-btn>
							</div>
						</div>
						<div>
							<h4 class="font-weight-medium" :class="hover ? 'primary--text' : ''">The Richland Center Shooping News and weekly shooper</h4>
						</div>
						<div class="mt-2">
							<p class="grey--text">Let one fifth i bring fly to divided face for bearing divide unto seed. Winged divided light Forth.</p>
						</div>
						<div>
							<v-btn text small class="py-5" :class="hover ? 'primary' : ''">
								<span>Read More</span>
								<v-icon :class="hover ? 'ml-2' : ''">mdi-arrow-right</v-icon>
							</v-btn>
						</div>
					</v-card>
				</v-hover>
			</v-col>
			<v-col cols="12" md="4" sm="4">
				<v-hover v-slot="{ hover }">
					<v-card flat>
						<v-img :src="getImg('blog3.png')"/>
						<div class="d-flex mt-3">
							<div class="d-flex">
								<p class="grey--text">By Admin</p>
							</div>
							<div class="d-flex ml-3">
								<v-btn text x-small class="d-flex" color="grey">
									<v-icon class="mr-1">mdi-chat-processing-outline</v-icon>
									<span>comments</span>
								</v-btn>
							</div>
						</div>
						<div>
							<h4 class="font-weight-medium" :class="hover ? 'primary--text' : ''">The Richland Center Shooping News and weekly shooper</h4>
						</div>
						<div class="mt-2">
							<p class="grey--text">Let one fifth i bring fly to divided face for bearing divide unto seed. Winged divided light Forth.</p>
						</div>
						<div>
							<v-btn text small class="py-5" :class="hover ? 'primary' : ''">
								<span>Read More</span>
								<v-icon :class="hover ? 'ml-2' : ''">mdi-arrow-right</v-icon>
							</v-btn>
						</div>
					</v-card>
				</v-hover>
			</v-col>
		</v-row>
	</div>
</template>

<script>
 export default{
 	methods: {
 	  getImg (img) {
 	   return require(`~/assets/images/blog/${img}`) 
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