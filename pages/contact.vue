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
              Contact Us
            </h1>
            <p class="grey--text">
              Home - Conact Us
            </p>  
          </v-col>
        </v-row>
    </v-parallax>
    <v-container>
      <GMap
        :cluster="{options: {styles: clusterStyle}}"
        :center="{lat: locations[0].lat, lng: locations[0].lng}"
        :options="{fullscreenControl: false, streetViewControl: false, mapTypeControl: false, zoomControl: true, gestureHandling: 'cooperative', styles: mapStyle}"
        :zoom="6"
      >
        <GMapMarker
          v-for="location in locations"
          :key="location.id"
          :position="{lat: location.lat, lng: location.lng}"
          :options="{icon: location === currentLocation ? pins.selected : pins.notSelected}"
          @click="currentLocation = location"
        >
          <GMapInfoWindow>
            <code>
              lat: {{ location.lat }},
              lng: {{ location.lng }}
            </code>
          </GMapInfoWindow>
        </GMapMarker>
      </GMap>
    </v-container>
    <v-container class="mb-5">
      <v-row align="center">
        <v-col cols="12" md='4' sm="6">
          <div>
            <v-row class="align-center">
              <v-col cols='4' md='2' sm="2">
                 <v-icon large color="primary">mdi-home</v-icon>
              </v-col>
              <v-col cols='8' md="7" sm="6" class="px-0">
                  <div>
                    <span class="font-weight-black">California United States</span>
                  </div>
                  <span class='date'>Santa monica bullevard</span>
              </v-col>
              </v-row>
          </div>
          <div>
            <v-row class="align-center">
              <v-col cols='4' md='2' sm="2">
                 <v-icon large color="primary">mdi-headphones</v-icon>
              </v-col>
              <v-col cols='8' md="7" sm="6" class="px-0">
                  <div>
                    <span class="font-weight-black">00 (440) 9865 562</span>
                  </div>
                  <span class='date'>Mon to Fri 9am to 6pm</span>
              </v-col>
              </v-row>
          </div>
          <div>
            <v-row class="align-center">
              <v-col cols='4' md='2' sm="2">
                 <v-icon large color="primary">mdi-email-outline</v-icon>
              </v-col>
              <v-col cols='8' md="7" sm="6" class="px-0">
                  <div>
                    <span class="font-weight-black">support@colorlib.com</span>
                  </div>
                  <span class='date'>Send us your query anytime!</span>
              </v-col>
              </v-row>
          </div>
        </v-col>
        <v-col cols="12" md='4' sm="6">
          <div>
            <v-text-field outlined dense solo flat placeholder="Enter Your Name"/>
          </div>
          <div>
            <v-text-field outlined dense solo flat placeholder="Enter Email Address"/>
          </div>
          <div>
            <v-text-field outlined dense solo flat placeholder="Enter Subject"/>
          </div>
        </v-col>
        <v-col cols="12" md="4">
          <div>
            <v-textarea outlined solo dense placeholder="Enter Message ...." flat/>
          </div>
        </v-col>
        <v-col cols='12' class="text-right">
          <v-btn color="primary" tile>Send Message</v-btn>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      currentLocation: {},
      locations: [
        {
          lat: 41.311081,
          lng: 69.240562
        },
        {
          lat: 45.815,
          lng: "15.9819"
        },
        {
          lat: "45.12",
          lng: "16.21"
        }
      ],
      pins: {
        selected:
          "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAMAAADXqc3KAAAApVBMVEUAAAD/AAD/AADxHCvyGyjzGDHoFy7vGSnwHi3wHSzsGi3uGivuHivrGyvsHCztGyrtHSzuHCvuHSzsHSzsHSvtHCvtHCrtGyvsHCvsHCvtHSztHCvtHCvtHCvuGyvtHCvtHSztGyvtHSvtHCvtHCztHCvsHCvtHCvtHCvtHCvtHCvtHCvtHCvtHCvtHCvtHCvtHCvtHCvtHCvtHCvtHCvtHCv///8Zo6fZAAAANXRSTlMAAQISExUWHyIjKDs8QVJVV1ppe3x+f4KHiJiZmpuxt7vDxMbHys7R4Ont7u/w8fLz9Pb7/qzXrqoAAAABYktHRDZHv4jRAAAAn0lEQVQYGaXBV5KCQABF0eeooxjGnDFnpc13/1uzi7JoQL/Gc/R/v931fr/u5JXSuBK61JVQe/Dy+FNM/kQkyMnpYRnfN1hdOVsgKEqeATZyzsBI1hg4yTkCQ1kj4CBnBQRFyTPAUs4Ay/i+werLKRFTUsyCyFxxFSJlJcx4mSnJuxG6FpTSJtRS2s8Ua5LRm+wOdll9UL3fq/qo2dQ3nvcVIgrnmsRBAAAAAElFTkSuQmCC",
        notSelected:
          "data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAABHElEQVR42uVVyw4BMRQdC98lsbPwG5YSH+BzWFtLZilh0oQgFh6J54IwBmGYtrfaBREdcTvDhpM0adrec3rb+7Csn8fRdrLg7VzBubhDzmHrudRuZ2KRs/miLd6AThfNaOTTGRFIsMm8bkSuXBeGoLVaGi0g39wLI4GTf1EjdE/+E1pAAGgEAenkb/tBo1vQFUDgBbSbny6al77uSQwB/6wJSNHoAo8xj30iaYMW4Lv9wfSTpc0eH6atXtE4TKWNUS4AY2hyddY4k/lwVEZncm9QilQuBGPwnp1B5GIXGi3P0eU0c7EqKrje5hU5d7fr2P2AEJIESkNqB1XJkvhI0/GrTuqZX619tLMF/VHlfnk5/0r7ZMvVWA3rr3AF6LIMZ7PmSlUAAAAASUVORK5CYII="
      },
      clusterStyle: [
        {
          url: "https://googlemaps.github.io/js-marker-clusterer/images/m2.png",
          width: 56,
          height: 56,
          textColor: "#fff"
        }
      ],
      mapStyle: [
        {
          featureType: "all",
          elementType: "labels.text.fill",
          stylers: [
            {
              color: "#ffffff"
            }
          ]
        },
        {
          featureType: "all",
          elementType: "labels.text.stroke",
          stylers: [
            {
              visibility: "on"
            },
            {
              color: "#3e606f"
            },
            {
              weight: 2
            },
            {
              gamma: 0.84
            }
          ]
        },
        {
          featureType: "all",
          elementType: "labels.icon",
          stylers: [
            {
              visibility: "off"
            }
          ]
        },
        {
          featureType: "administrative",
          elementType: "geometry",
          stylers: [
            {
              weight: 0.6
            },
            {
              color: "#313536"
            }
          ]
        },
        {
          featureType: "landscape",
          elementType: "geometry",
          stylers: [
            {
              color: "#44a688"
            }
          ]
        },
        {
          featureType: "poi",
          elementType: "geometry",
          stylers: [
            {
              color: "#13876c"
            }
          ]
        },
        {
          featureType: "poi.attraction",
          elementType: "geometry.stroke",
          stylers: [
            {
              color: "#f5e4e4"
            },
            {
              visibility: "off"
            }
          ]
        },
        {
          featureType: "poi.attraction",
          elementType: "labels",
          stylers: [
            {
              visibility: "on"
            },
            {
              lightness: "14"
            }
          ]
        },
        {
          featureType: "poi.park",
          elementType: "geometry",
          stylers: [
            {
              color: "#13876c"
            },
            {
              visibility: "simplified"
            }
          ]
        },
        {
          featureType: "road",
          elementType: "geometry",
          stylers: [
            {
              color: "#067372"
            },
            {
              lightness: "-20"
            }
          ]
        },
        {
          featureType: "transit",
          elementType: "geometry",
          stylers: [
            {
              color: "#357374"
            }
          ]
        },
        {
          featureType: "water",
          elementType: "geometry",
          stylers: [
            {
              color: "#004757"
            }
          ]
        }
      ]
    };
  },
  methods: {
      getImageUrl (img){
        return require(`~/assets/images/blog/${img}`)
      }
    }
};
</script>

<style lang="scss">
* {
  font-family: Arial, "Helvetica Neue", Helvetica, sans-serif;
}

h1 {
  color: #206569;
  margin-bottom: 5px;
  & + p {
    margin-top: 0;
    font-size: 16px;
    a {
      color: #206569;
    }
  }
}

span,
p,
a {
  color: #206569;
  font-size: 16px;
}

.GMap,
p {
  margin-top: 30px;
}

.GMap__Wrapper {
  width: 100%;
  height: 400px;
}
</style>