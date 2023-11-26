<template>
    <v-sheet
    class="d-flex align-center justify-center flex-wrap text-center mx-auto px-4 mt-16"
    elevation="4"
    height="100vh"
    rounded
    max-width="80%"
    width="100%"
  >
    <div>
      <h2 class="titulo text-h2 font-weight-black text-orange">
        Empresa en un mundo digital
      </h2>

      <div class="subtitulo text-h4 font-weight-medium mb-8 mt-8">
        Si estás aqui es porque...
      </div>

      <p class="texto text-h6 mb-8 mt-8">
        valoras la excelencia en la presencia digital de tu negocio. En nuestra plataforma, te ofrecemos no solo servicios de diseño web vanguardistas, sino también soluciones tecnológicas personalizadas para potenciar el rendimiento de tu empresa. Desde la implementación de bases de datos hasta la creación de portales especializados, nuestro compromiso es impulsar tu éxito en línea. Con enfoque en el posicionamiento web y SEO, nos esforzamos por llevar tu presencia digital a nuevas alturas. ¡Descubre cómo podemos transformar tu visión en una realidad digital impactante y efectiva!
      </p>

      <nuxt-link to="/servicios"><v-btn color="orange" size="x-large" elevation="4">Descubrir</v-btn></nuxt-link>
    </div>
  </v-sheet>
    <div class="main">
        <v-container class="mt-16">
            <v-row justify="space-around">
              <!-- <v-col
                v-for="elevation in elevations"
                :key="elevation"
                md="6"
                col="6"
              >
                <v-sheet
                  class="pa-12"
                  color="grey-lighten-3"
                >
                  <v-sheet
                    :elevation="elevation"
                    class="mx-auto"
                    height="100"
                    width="100"
                  ></v-sheet>
                </v-sheet>
              </v-col> -->
              <v-col>
                <v-card
                class="mx-auto"
                max-width="344"
              >
                <v-img
                  src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                  height="200px"
                  cover
                ></v-img>
            
                <v-card-title>
                  Top western road trips
                </v-card-title>
            
                <v-card-subtitle>
                  1,000 miles of wonder
                </v-card-subtitle>
            
                <v-card-actions>
                  <v-btn
                    color="orange-lighten-2"
                    variant="text"
                  >
                    Explore
                  </v-btn>
            
                  <v-spacer></v-spacer>
            
                  <v-btn
                    :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'"
                    @click="show = !show"
                  ></v-btn>
                </v-card-actions>
            
                <v-expand-transition>
                  <div v-show="show">
                    <v-divider></v-divider>
            
                    <v-card-text>
                      I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape.
                    </v-card-text>
                  </div>
                </v-expand-transition>
              </v-card>
              </v-col>
              <v-col>
              <v-card
              class="mx-auto"
              max-width="344"
            >
              <v-img
                src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
                height="200px"
                cover
              ></v-img>
          
              <v-card-title>
                Top western road trips
              </v-card-title>
          
              <v-card-subtitle>
                1,000 miles of wonder
              </v-card-subtitle>
          
              <v-card-actions>
                <v-btn
                  color="orange-lighten-2"
                  variant="text"
                >
                  Explore
                </v-btn>
          
                <v-spacer></v-spacer>
          
                <v-btn
                  :icon="show ? 'mdi-chevron-up' : 'mdi-chevron-down'"
                  @click="show = !show"
                ></v-btn>
              </v-card-actions>
          
              <v-expand-transition>
                <div v-show="show">
                  <v-divider></v-divider>
          
                  <v-card-text>
                    I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape.
                  </v-card-text>
                </div>
              </v-expand-transition>
            </v-card>
        </v-col>
            </v-row>
          </v-container>
    </div>
</template>

<style>
.main {
    height: 100vh;
}

@media screen and (max-width: 1100px) {
  .titulo {
    font-size: 2rem !important;
    line-height: 2rem;
  }
  .subtitulo {
    font-size: 1.4rem !important;
  }
  .texto {
    font-size: 1rem !important;
    line-height: 1.2rem;
  }
}
</style>

<script>
  export default {
    data: () => ({ 
        show: false,
    }),
  }
</script>