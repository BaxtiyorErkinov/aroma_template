<template>
	<div>
		<v-row>
			<v-col cols="12" md="8" sm='12'>
				<v-card flat class="mb-5">
					<v-row>
						<v-col cols="12">
							<v-img :src="getImg('feature-img1.jpg')"/>
						</v-col>
						<v-col cols="4" class="text-center mt-1">
							<div class=""><p class="my-0 font">Food<span class="primary--text"> Technology</span></p></div>
							<div class="pl-2"><p class="my-0 font">Politics, Lifestyle</p></div>
							<v-row class="mt-3">
								<v-hover v-slot="{ hover }">
									<v-col cols="12" class="py-1 caption" :class="hover ? 'primary--text' : 'grey--text'">
									Mark wiens
									<v-icon class="ml-4" :color="hover ? 'primary' : ''">mdi-account-outline</v-icon>
								</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="12" class=" py-1 caption" :class="hover ? 'primary--text' : 'grey--text'">
									12 Dec, 2017
									<v-icon class="ml-2" :color="hover ? 'primary' : ''">mdi-calendar</v-icon>
								</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="12" class=" py-1 caption" :class="hover ? 'primary--text' : 'grey--text'">
									1.2M Views
									<v-icon class="ml-4" :color="hover ? 'primary' : ''">mdi-eye</v-icon>
								</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="12" class="py-1 caption" :class="hover ? 'primary--text' : 'grey--text'">
									06 Comments
									<v-icon class="ml-2" :color="hover ? 'primary' : ''">mdi-comment-outline</v-icon>
								</v-col>
								</v-hover>
							</v-row>
						</v-col>
						<v-col cols="8" class="py-0 px-0">
							<v-hover v-slot="{ hover }">
								<v-card-title class="font-weight-black text-h5" :class="hover ? 'primary--text' : ''">Astronomy Binoculars A Great Alternative</v-card-title>
							</v-hover>
							<div class="px-3 mr-3">
								<p class="grey--text subtitle">MCSE boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction.</p>
							</div>
							<div class="px-3 mr-3">
								<p class="grey--text subtitle">Boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction of the camp price. However, who has the willpower to actually sit through a self-imposed MCSE training. who has the willpower to actually sit through a self-imposed</p>
							</div>
							<div class="px-3 mr-3">
								<p class="grey--text subtitle">Boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction of the camp price. However, who has the willpower to actually sit through a self-imposed MCSE training. who has the willpower to actually sit through a self-imposed</p>
							</div>
						</v-col>
						<v-col cols="12" class="mt-2">
							<v-sheet class="pt-5 pb-1 px-3 box" rounded color="#fff">
								<p class="font-italic font-weight-light">MCSE boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction of the camp price. However, who has the willpower to actually sit through a self-imposed MCSE training.</p>
							</v-sheet>
						</v-col>
						<v-col cols="6">
							<v-img :src="itemImg('post-img1.jpg')"/>
						</v-col>
						<v-col cols="6">
							<v-img :src="itemImg('post-img2.jpg')"/>
						</v-col>
						<v-col cols=12>
							<p class="grey--text">MCSE boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction of the camp price. However, who has the willpower.</p>
						</v-col>
						<v-col cols="12">
							<p class="grey--text">MCSE boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction of the camp price. However, who has the willpower.</p>
						</v-col>
						<v-col cols="12">
							<v-divider />
						</v-col>
						<v-col cols="12" md="6" sm='6'>
							<v-row>
								<v-col cols='2' class="mr-2">
									<img :src="itemImg('prev.jpg')"/>
								</v-col>
								<v-col cols="8">
									<div>
										<p class='mb-0 grey--text'>Prev Post</p>
										<p class="mt-2 font-weight-medium">Space The Final Frontier</p>
									</div>
								</v-col>
							</v-row>
						</v-col>
						<v-col cols="12" md='6' sm="6">
							<v-row>
								<v-col cols="8" class="text-right">
									<div>
										<p class='mb-0 grey--text'>Next Post</p>
										<p class="mt-2 font-weight-medium">Telescopes 101</p>
									</div>
								</v-col>
								<v-col cols='2' class="ml-2">
									<img :src="itemImg('next.jpg')"/>
								</v-col>
							</v-row>
						</v-col>
						<v-col cols='12'>
							<v-card flat color='#f8f9fa' class='pa-5'>
								<v-col cols="12" class='text-center'>
									<h3 class='font-weight-medium'>05 Comments</h3>
								</v-col>
								<v-col cols='12' class="py-2">
			         				<v-card class="py-1 px-5" tile flat color='#f8f9fa'>
					          			<v-row class="align-center">
					          				<v-col cols='4' md='2' sm="2">
					          					<v-avatar size="60" tile>
					          						<img :src="itemImg('c1.jpg')" />
					          					</v-avatar>
					          				</v-col>
					          				<v-col cols='8' md="5" sm="5" class="px-0">
					          					<div>
					          						<span class="font-weight-black text">Blake Ruiz</span>
					          					</div>
					          						<span class='date'>December 4, 2017 at 3:12 pm</span>
					          				</v-col>
					          				<v-col cols="5" class=" d-flex justify-end">
					          					<v-btn small outlined text>Reply</v-btn>
					          				</v-col>
					          				<v-col cols="12" class="pa-1">
					          					<p class="grey--text">
					          						Never say goodbye till the end comes!
					          					</p>
					          				</v-col>
					          			</v-row>
			          				</v-card>
			         			</v-col>
			         			<v-col cols='12' class="py-2">
			         				<v-card class="py-1 px-md-5 ml-md-7" tile flat color='#f8f9fa'>
					          			<v-row class="align-center">
					          				<v-col cols='4' md='2' sm="2">
					          					<v-avatar size="60" tile>
					          						<img :src="itemImg('c2.jpg')" />
					          					</v-avatar>
					          				</v-col>
					          				<v-col cols='8' md="5" sm="5" class="px-0">
					          					<div>
					          						<span class="font-weight-black text">Elsie Cunningham</span>
					          					</div>
					          						<span class='date'>December 4, 2017 at 3:12 pm</span>
					          				</v-col>
					          				<v-col cols="5" class=" d-flex justify-end">
					          					<v-btn small outlined text>Reply</v-btn>
					          				</v-col>
					          				<v-col cols="12" class="pa-1">
					          					<p class="grey--text">
					          						Never say goodbye till the end comes!
					          					</p>
					          				</v-col>
					          			</v-row>
			          				</v-card>
			         			</v-col>
			         			<v-col cols='12' class="py-2">
			         				<v-card class="py-1 px-md-5 ml-md-7" tile flat color='#f8f9fa'>
					          			<v-row class="align-center">
					          				<v-col cols='4' md='2' sm="2">
					          					<v-avatar size="60" tile>
					          						<img :src="itemImg('c3.jpg')" />
					          					</v-avatar>
					          				</v-col>
					          				<v-col  cols='8' md="5" sm="5" class="px-0">
					          					<div>
					          						<span class="font-weight-black text">Annie Stephens</span>
					          					</div>
					          						<span class='date'>December 4, 2017 at 3:12 pm</span>
					          				</v-col>
					          				<v-col cols="5" class=" d-flex justify-end">
					          					<v-btn small outlined text>Reply</v-btn>
					          				</v-col>
					          				<v-col cols="12" class="pa-1">
					          					<p class="grey--text">
					          						Never say goodbye till the end comes!
					          					</p>
					          				</v-col>
					          			</v-row>
			          				</v-card>
			         			</v-col>
			         			<v-col cols='12' class="py-2">
			         				<v-card class="py-1 px-md-5" tile flat color='#f8f9fa'>
					          			<v-row class="align-center">
					          				<v-col cols='4' md='2' sm="2">
					          					<v-avatar size="60" tile>
					          						<img :src="itemImg('c4.jpg')" />
					          					</v-avatar>
					          				</v-col>
					          				<v-col  cols='8' md="5" sm="5" class="px-0">
					          					<div>
					          						<span class="font-weight-black text">Maria Luna</span>
					          					</div>
					          						<span class='date'>December 4, 2017 at 3:12 pm</span>
					          				</v-col>
					          				<v-col cols="5" class=" d-flex justify-end">
					          					<v-btn small outlined text>Reply</v-btn>
					          				</v-col>
					          				<v-col cols="12" class="pa-1">
					          					<p class="grey--text">
					          						Never say goodbye till the end comes!
					          					</p>
					          				</v-col>
					          			</v-row>
			          				</v-card>
			         			</v-col>
			         			<v-col cols='12' class="py-2">
			         				<v-card class="py-1 px-md-5" tile flat color='#f8f9fa'>
					          			<v-row class="align-center">
					          				<v-col cols='4' md='2' sm="2">
					          					<v-avatar size="60" tile>
					          						<img :src="itemImg('c5.jpg')" />
					          					</v-avatar>
					          				</v-col>
					          				<v-col cols='8' md="5" sm="5" class="px-0">
					          					<div>
					          						<span class="font-weight-black text">Ina Hayes</span>
					          					</div>
					          						<span class='date'>December 4, 2017 at 3:12 pm</span>
					          				</v-col>
					          				<v-col cols="5" class=" d-flex justify-end">
					          					<v-btn small outlined text>Reply</v-btn>
					          				</v-col>
					          				<v-col cols="12" class="pa-1">
					          					<p class="grey--text">
					          						Never say goodbye till the end comes!
					          					</p>
					          				</v-col>
					          			</v-row>
			          				</v-card>
			         			</v-col>
							</v-card>
						</v-col>
						<v-col cols='12' class="mb-3">
							<v-card color="#f8f9fa" flat class="pa-5">
								<v-row>
									<v-col cols='12' class="text-center font-weight-medium">Leave a Reply</v-col>
									<v-col cols="6" class="py-0 mt-3">
										<v-text-field outlined solo dense flat placeholder="Enter Name"/>
									</v-col>
									<v-col cols="6" class="py-0 mt-3">
										<v-text-field outlined solo dense flat placeholder="Enter email address"/>
									</v-col>
									<v-col cols="12" class='py-0'>
										<v-text-field outlined solo dense flat placeholder="Subject"/>
									</v-col>
									<v-col cols='12' class="py-0">
										<v-textarea placeholder="Message" outlined solo flat />
									</v-col>
									<v-col cols="12" class="py-0 text-center mb-3">
										<v-btn color="primary" x-large>Post Comment</v-btn>
									</v-col>
								</v-row>
							</v-card>
						</v-col>
					</v-row>
				</v-card>
			</v-col>
			<v-col cols="12" md="4">
					<v-card color="#f1f6f7" flat class="pa-6">
						<v-row>
							<v-col cols="12" class="pb-1">
								<v-text-field outlined rounded dense background-color="primary" dark height="20" append-icon="mdi-magnify" placeholder="Search Posts"/>
							</v-col>
							<v-col cols="12" class="pt-0">
								<v-divider />
							</v-col>
							<v-col cols="12" class="text-center">
								<v-avatar size="120">
									<v-img :src="itemImg('author.png')"/>
								</v-avatar>
							</v-col>
							<v-col cols="12" class="text-center pb-0">
								<h3 class="font-weight-medium">Charlie Barber</h3>
							</v-col>
							<v-col cols="12" class="text-center pt-0">
								<p class="grey--text subtitle">Senior blog writer</p>
							</v-col>
							<v-col cols="12" class="pt-0">
								<v-row class="text-center">
									<v-col cols="12" class="pt-0 text">
										<v-icon class="mr-3">mdi-facebook</v-icon>
										<v-icon>mdi-twitter</v-icon>
										<v-icon class="ml-3">mdi-github</v-icon>
									</v-col>
								</v-row>
							</v-col>
							<v-col cols="12" class="px-3 text-center">
								<p class="grey--text">Boot camps have its supporters andit sdetractors. Some people do not understand why you should have to spend money on boot camp when you can get. Boot camps have itssuppor ters andits detractors.</p>
							</v-col>
							<v-col cols="12">
								<v-divider />
							</v-col>
							<v-col cols="12" class='text-center'>
								<v-btn color='primary' depressed tile large width="100%">
									Popular Posts
								</v-btn>
							</v-col>
							<v-col cols='12' class="pb-0">
								<v-container>							
									<div>
										<v-row>
											<v-col cols="5">
												<v-img :src="getPostImage('post1.jpg')" height="60" width="100"></v-img>
											</v-col>
											<v-col cols="7" class="px-0">
												<h5 class="font-weight-black">Space The Final Frontier</h5>
												<p class="mt-1 grey--text caption">02 Hours ago</p>
											</v-col>
										</v-row>
									</div>
								</v-container>
							</v-col>
							<v-col cols='12' class='pb-0'>
								<v-container>							
									<div>
										<v-row>
											<v-col cols="5">
												<v-img :src="getPostImage('post2.jpg')" height="60" width="100"></v-img>
											</v-col>
											<v-col cols="7" class="px-0">
												<h5 class="font-weight-black">The Amazing Hubble</h5>
												<p class="mt-1 grey--text caption">02 Hours ago</p>
											</v-col>
										</v-row>
									</div>
								</v-container>
							</v-col>
							<v-col cols='12' class="pb-0">
								<v-container>							
									<div>
										<v-row>
											<v-col cols="5">
												<v-img :src="getPostImage('post3.jpg')" height="60" width="100"></v-img>
											</v-col>
											<v-col cols="7" class="px-0">
												<h5 class="font-weight-black">Astronomy Or Astrology</h5>
												<p class="mt-1 grey--text caption">02 Hours ago</p>
											</v-col>
										</v-row>
									</div>
								</v-container>
							</v-col>
							<v-col cols='12' class="pb-0">
								<v-container>							
									<div>
										<v-row>
											<v-col cols="5">
												<v-img :src="getPostImage('post4.jpg')" height="60" width="100"></v-img>
											</v-col>
											<v-col cols="7" class="px-0">
												<h5 class="font-weight-black">Asteroids telescope</h5>
												<p class="mt-1 grey--text caption">02 Hours ago</p>
											</v-col>
										</v-row>
									</div>
								</v-container>
							</v-col>
							<v-col cols='12'>
								<v-divider />
							</v-col>
							<v-col cols="12">
								<v-img :src="itemImg('add.jpg')"/>
							</v-col>
							<v-col cols='12'>
								<v-divider />
							</v-col>
							<v-col cols="12" class="text-center mb-4">
								<v-btn color='primary' tile width="100%">Post Categories</v-btn>
							</v-col>
							<v-col cols='12'>
							<v-hover v-slot="{ hover }">
								<v-row class="grey--text">
									<v-col cols='10' :class="hover ? 'primary--text' : ''">
										Technology
									</v-col>
									<v-col cols='2' :class="hover ? 'primary--text' : ''">
										37
									</v-col>
									<v-col cols='12'>
										<v-divider :class="hover ? 'primary' : ''"/>
									</v-col>
								</v-row>
							</v-hover>
							<v-hover v-slot="{ hover }">
								<v-row class="grey--text">
									<v-col cols='10' :class="hover ? 'primary--text' : ''">
										Lifestyle
									</v-col>
									<v-col cols='2' :class="hover ? 'primary--text' : ''">
										24
									</v-col>
									<v-col cols='12'>
										<v-divider :class="hover ? 'primary' : ''"/>
									</v-col>
								</v-row>
							</v-hover>
							<v-hover v-slot="{ hover }">
								<v-row class="grey--text">
									<v-col cols='10' :class="hover ? 'primary--text' : ''">
										Fashion
									</v-col>
									<v-col cols='2' :class="hover ? 'primary--text' : ''">
										10
									</v-col>
									<v-col cols='12'>
										<v-divider :class="hover ? 'primary' : ''"/>
									</v-col>
								</v-row>
							</v-hover>
							<v-hover v-slot="{ hover }">
								<v-row class="grey--text">
									<v-col cols='10' :class="hover ? 'primary--text' : ''">
										Art
									</v-col>
									<v-col cols='2' :class="hover ? 'primary--text' : ''">
										12
									</v-col>
									<v-col cols='12'>
										<v-divider :class="hover ? 'primary' : ''"/>
									</v-col>
								</v-row>
							</v-hover>
							<v-hover v-slot="{ hover }">
								<v-row class="grey--text">
									<v-col cols='10' :class="hover ? 'primary--text' : ''">
										Food
									</v-col>
									<v-col cols='2' :class="hover ? 'primary--text' : ''">
										32
									</v-col>
									<v-col cols='12'>
										<v-divider :class="hover ? 'primary' : ''"/>
									</v-col>
								</v-row>
							</v-hover>
							<v-hover v-slot="{ hover }">
								<v-row class="grey--text">
									<v-col cols='10' :class="hover ? 'primary--text' : ''">
										Architecture
									</v-col>
									<v-col cols='2' :class="hover ? 'primary--text' : ''">
										18
									</v-col>
									<v-col cols='12'>
										<v-divider :class="hover ? 'primary' : ''"/>
									</v-col>
								</v-row>
							</v-hover>
							<v-hover v-slot="{ hover }">
								<v-row class="grey--text">
									<v-col cols='10' :class="hover ? 'primary--text' : ''">
										Adventure
									</v-col>
									<v-col cols='2' :class="hover ? 'primary--text' : ''">
										20
									</v-col>
									<v-col cols='12'>
										<v-divider :class="hover ? 'primary' : ''"/>
									</v-col>
								</v-row>
							</v-hover>
							</v-col>
							<v-col cols='12'>
								<v-btn tile color="primary" width="100%">Newsletter</v-btn>
							</v-col>
							<v-col cols='12' class="px-7 text-center">
								<p class="grey--text subtitle">Here, I focus on a range of items and features that we use in life without giving them a second thought.</p>
							</v-col>
							<v-col cols='12' class="px-7 pb-0">
								<v-row>
									<v-col cols='6' class="px-0">
										<v-text-field dense prepend-inner-icon="mdi-email" outlined flat solo filled placeholder="Email Address"/>
									</v-col>
									<v-col cols="4">
										<v-btn depressed height="40" color="primary">Subscribe</v-btn>
									</v-col>
								</v-row>
							</v-col>
							<v-col cols='12' class="text-center pt-0">
								<p class="caption">You can unsubscribe at any time</p>
							</v-col>
							<v-col cols="12">
								<v-divider />
							</v-col>
							<v-col cols="12">
								<v-btn width="100%" depressed color="primary">Tag Clouds</v-btn>
							</v-col>
							<v-col cols="12">
								<v-btn small depressed tile color="#fff" class="mb-1"><span class="caption">Technology</span></v-btn>
								<v-btn small depressed tile color="#fff" class="mb-1"><span class="caption">Fashion</span></v-btn>
								<v-btn small depressed tile color="#fff" class="mb-1"><span class="caption">Architecture</span></v-btn>
								<v-btn small depressed tile color="#fff" class="mb-1"><span class="caption">Food</span></v-btn>
								<v-btn small depressed tile color="#fff" class="mb-1"><span class="caption">Adventure</span></v-btn>
							</v-col>
						</v-row>
					</v-card>
			</v-col>
		</v-row>
	</div>
</template>

<script>
	export default{
		data(){
			return{

			}
		},
		methods: {
		  getImg (img) {
		    return require(`~/assets/images/blog/${img}`)
		  },
		  itemImg(img){
		  	return require(`~/assets/images/blog/${img}`)
		  },
		  getPostImage(img){
				return require(`~/assets/images/blog/popular-post/${img}`)
			}
		}
	}
</script>


<style scoped> 
	.subtitle{
		font-size: 15px;
	}
	.box{
		box-shadow: rgba(0, 0, 0, 0.1) 0px 20px 25px -5px, rgba(0, 0, 0, 0.04) 0px 10px 10px -5px;
		border-radius: 5px;
		font-size: 14px; 
		color: grey;
	}
	.text{
		font-family: Ubuntu;
	}
	.date{
		font-size: 14px;
		color: grey;
	}
</style>