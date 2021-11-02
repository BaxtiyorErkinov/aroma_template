<template>
	<div>
		<v-row class="mb-5">
			<v-col md="4" sm='6'>
				<v-card>
					<v-img :src="getImageUrl('cat-post-3.jpg')" class="pa-5 align-center">
						<v-card flat color="rgba(0,0,0, .5)" class="pa-10">
							<v-row class="text-center white--text">
								<v-col cols="12">
									<h3>SOCIAL LIFE</h3>
								</v-col>
								<v-col cols='12'>
									<v-divider color="white"/>
								</v-col>
								<v-col cols="12">
									<p>Enjoy your social life together</p>
								</v-col>
							</v-row>
						</v-card>
					</v-img>
				</v-card>
			</v-col>
			<v-col md="4" sm="6">
				<v-card>
					<v-img :src="getImageUrl('cat-post-2.jpg')" class="pa-5 align-center">
						<v-card flat color="rgba(0,0,0, .5)" class="pa-10">
							<v-row class="text-center white--text">
								<v-col cols="12">
									<h3>POLITICS</h3>
								</v-col>
								<v-col cols='12'>
									<v-divider color="white"/>
								</v-col>
								<v-col cols="12">
									<p>Be a part of politics</p>
								</v-col>
							</v-row>
						</v-card>
					</v-img>
				</v-card>
			</v-col>
			<v-col md="4" sm="12">
				<v-card>
					<v-img :src="getImageUrl('cat-post-1.jpg')" class="pa-5 align-center">
						<v-card flat color="rgba(0,0,0, .5)" class="pa-10">
							<v-row class="text-center white--text">
								<v-col cols="12">
									<h3>FOOD</h3>
								</v-col>
								<v-col cols='12'>
									<v-divider color="white"/>
								</v-col>
								<v-col cols="12">
									<p>Let the food be finished</p>
								</v-col>
							</v-row>
						</v-card>
					</v-img>
				</v-card>
			</v-col>
		</v-row>
		<v-row>
			<v-col cols='12' md="8" sm="12">
				<v-col cols="12">
					<v-row>
						<v-col cols="12" md="4" sm="4" class="text-right">
							<div><p class="my-0 font">Food<span class="primary--text"> Technology</span></p></div>
							<div class="pl-2"><p class="my-0 font">Politics, Lifestyle</p></div>
							<v-row class="mt-3">
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">Mark wiens</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-account-outline</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">12 Dec, 2017</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-calendar</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">1.2M Views</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-eye</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">06 Comments</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-comment-outline</v-icon></v-col>
								</v-hover>

							</v-row>
						</v-col>
						<v-col cols="12" md="8" sm="8">
							<v-card>
								<v-img :src="cardsImg('m-blog-1.jpg')"/>
								<v-card-title class="font-weight-black">Astronomy Binoculars A Great Alternative</v-card-title>
								<div class="pa-3">
									<p class="grey--text my-0">MCSE boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction.</p>
								</div>
								<div class="pa-3">
									<v-btn outlined depressed color="grey">View more</v-btn>
								</div>
							</v-card>
						</v-col>
					</v-row>
				</v-col>	
				<v-col cols="12">
					<v-row>
						<v-col cols="12" md="4" sm="4" class="text-right">
							<div><p class="my-0 font">Food<span class="primary--text"> Technology</span></p></div>
							<div class="pl-2"><p class="my-0 font">Politics, Lifestyle</p></div>
							<v-row class="mt-3">
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">Mark wiens</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-account-outline</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">12 Dec, 2017</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-calendar</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">1.2M Views</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-eye</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">06 Comments</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-comment-outline</v-icon></v-col>
								</v-hover>

							</v-row>
						</v-col>
						<v-col cols="12" md="8" sm="8">
							<v-card>
								<v-img :src="cardsImg('m-blog-2.jpg')"/>
								<v-card-title class="font-weight-black">The Basics Of Buying A Telescope</v-card-title>
								<div class="pa-3">
									<p class="grey--text my-0">MCSE boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction.</p>
								</div>
								<div class="pa-3">
									<v-btn outlined depressed color='grey'>View more</v-btn>
								</div>
							</v-card>
						</v-col>
					</v-row>
				</v-col>
				<v-col cols="12">
					<v-row>
						<v-col cols="12" md="4" sm="4" class="text-right">
							<div><p class="my-0 font">Food<span class="primary--text"> Technology</span></p></div>
							<div class="pl-2"><p class="my-0 font">Politics, Lifestyle</p></div>
							<v-row class="mt-3">
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">Mark wiens</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-account-outline</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">12 Dec, 2017</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-calendar</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">1.2M Views</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-eye</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">06 Comments</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-comment-outline</v-icon></v-col>
								</v-hover>

							</v-row>
						</v-col>
						<v-col cols="12" md="8" sm="8">
							<v-card>
								<v-img :src="cardsImg('m-blog-3.jpg')"/>
								<v-card-title class="font-weight-black">The Glossary Of Telescopes</v-card-title>
								<div class="pa-3">
									<p class="grey--text my-0">MCSE boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction.</p>
								</div>
								<div class="pa-3">
									<v-btn outlined depressed color='grey'>View more</v-btn>
								</div>
							</v-card>
						</v-col>
					</v-row>
				</v-col>
				<v-col cols="12">
					<v-row>
						<v-col cols="12" md="4" sm="4"  class="text-right">
							<div><p class="my-0 font">Food<span class="primary--text"> Technology</span></p></div>
							<div class="pl-2"><p class="my-0 font">Politics, Lifestyle</p></div>
							<v-row class="mt-3">
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">Mark wiens</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-account-outline</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">12 Dec, 2017</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-calendar</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">1.2M Views</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-eye</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">06 Comments</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-comment-outline</v-icon></v-col>
								</v-hover>

							</v-row>
						</v-col>
						<v-col cols="12" md="8" sm='8'>
							<v-card>
								<v-img :src="cardsImg('m-blog-4.jpg')"/>
								<v-card-title class="font-weight-black">The Night Sky</v-card-title>
								<div class="pa-3">
									<p class="grey--text my-0">MCSE boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction.</p>
								</div>
								<div class="pa-3">
									<v-btn outlined depressed color="grey">View more</v-btn>
								</div>
							</v-card>
						</v-col>
					</v-row>
				</v-col>
				<v-col cols="12">
					<v-row>
						<v-col cols="12" md="4" sm="4" class="text-right">
							<div><p class="my-0 font">Food<span class="primary--text"> Technology</span></p></div>
							<div class="pl-2"><p class="my-0 font">Politics, Lifestyle</p></div>
							<v-row class="mt-3">
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">Mark wiens</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-account-outline</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">12 Dec, 2017</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-calendar</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">1.2M Views</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-eye</v-icon></v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="10" class="text-right py-1" :class="hover ? 'primary--text' : 'grey--text'">06 Comments</v-col>
								</v-hover>
								<v-hover v-slot="{ hover }">
									<v-col cols="1" class="py-1"><v-icon>mdi-comment-outline</v-icon></v-col>
								</v-hover>

							</v-row>
						</v-col>
						<v-col cols="12" md="8" sm="8">
							<v-card>
								<v-img :src="cardsImg('m-blog-5.jpg')"/>
								<v-card-title class="font-weight-black">Telescopes 101</v-card-title>
								<div class="pa-3">
									<p class="grey--text my-0">MCSE boot camps have its supporters and its detractors. Some people do not understand why you should have to spend money on boot camp when you can get the MCSE study materials yourself at a fraction.</p>
								</div>
								<div class="pa-3">
									<v-btn outlined depressed color="grey">View more</v-btn>
								</div>
							</v-card>
						</v-col>
					</v-row>
				</v-col>
			</v-col>
			<v-col cols='12' md="4" sm="12">
				<v-col cols="12">
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
									<v-img :src="authorImg('author.png')"/>
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
								<v-img :src="authorImg('add.jpg')"/>
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
			</v-col>
		</v-row>
		<v-row class="mb-5">
			<v-col cols="12">
				<v-pagination
					v-model="page"
				    :length="6"
				></v-pagination>
			</v-col>
		</v-row>
	</div>
</template>
<script>
	export default{
		data(){
			return{
				postItems: [
					{
						id: 1,
						title: 'Technology',
						count: '37'
					},
					{
						id: 2,
						title: 'Lifestyle',
						count: '24'
					},
					{
						id: 1,
						title: 'Fashion',
						count: '59'
					},
					{
						id: 1,
						title: 'Art',
						count: '29'
					},
					{
						id: 1,
						title: 'Food',
						count: '15'
					},
					{
						id: 1,
						title: 'Architecture',
						count: '09'
					},
					{
						id: 1,
						title: 'Adventure',
						count: '44'
					}
				],
				page: 2,
			}
		},
		methods: {
			getImageUrl (img){
				return require(`~/assets/images/blog/cat-post/${img}`)
			},
			cardsImg(img){
				return require(`~/assets/images/blog/main-blog/${img}`)
			},
			authorImg(img){
				return require(`~/assets/images/blog/${img}`)
			},
			getPostImage(img){
				return require(`~/assets/images/blog/popular-post/${img}`)
			}
		}
	}
</script>

<style scoped>
	.font{
		font-family: Ubuntu;
		font-size: 16px;
	}
	.subtitle{
		font-size: 14px;
	}
</style>