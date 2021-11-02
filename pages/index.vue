<template>
  <div>
    <v-row>
      <v-col cols="1" md="4" sm="2">
        <div class="first-block">
          <img src="@/assets/images/home/hero-banner.png" class="hero-banner hidden-sm-and-down"/>
        </div>
      </v-col>
      <v-col cols="10" md="8" sm="10">
        <div class="second-block pa-md-16 pa-sm-2">
          <v-container class="pa-md-16">
            <v-card flat color="#f8f9fa">
              <v-row>
                <v-col cols="12" md="8">
                  <div class="px-3 py-3 item">
                    <h4 class="grey--text font-weight-medium">Shop is fun</h4>
                  </div> 
                  <div class="px-6">
                    <h1 class="hero-text">BROWSE OUR PREMIUM PRODUCT</h1>
                  </div>
                </v-col>
                <v-col cols="12" md="9">
                  <div class="px-6 item">                  
                    <p>
                      Us which over of signs divide dominion deep fill bring they're meat beho upon own earth without morning over third. Their male dry. They are great appear whose land fly grass.
                    </p>
                  </div>
                </v-col>
                <v-col cols="12">
                  <div class="px-6 item">
                    <v-btn x-large rounded color="primary" class="white--text">Browse Now</v-btn>
                  </div>
                </v-col>
              </v-row>
            </v-card>
          </v-container>
        </div>
      </v-col>
    </v-row>
    <div>
      <Home-Cards />
    </div>
    <v-container class="mt-5">
      <Home-Cards-second />
    </v-container>
    <div>
      <Home-paralax />
    </div>
    <div>
      <slide-group />
    </div>
    <v-container>
      <Home-News />
    </v-container>
    <v-container>
      <Home-form />
    </v-container>
  </div>
</template>

<style scoped>
  .first-block{
    width: 110%;
    height: 93.5vh;
    background: #6610f2;
  }
  .second-block{
    width: 100%;
    background: #f8f9fa;
  }
  .hero-banner{
    width: 400px;
    height: 500px;
    position: absolute;
    top: 98px;
    left: 170px;
  }
  .hero-text{
    font-size: 35px;
  }
/*  .item{
    width: 100%;
  }*/
  @media only screen 
  and (min-device-width: 360px) 
  and (max-device-width: 640px) { 
  .first-block{
    width: 100%;
    height: 78vh;
    background: #6610f2;
  } 
}
@media only screen 
  and (min-device-width: 768px) 
  and (max-device-width: 1024px){
  .first-block{
    width: 30vh;
    height: 37vh;
    background: #6610f2;
  }
}
@media only screen 
  and (min-device-width: 360px) 
  and (max-device-width: 640px){
  .first-block{
    width: 100%;
    height: 78vh;
    background: #6610f2;
  } 
  }

</style>
