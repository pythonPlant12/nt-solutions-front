<template>
<div class="toda-pagina">
	<div class="primera-pantalla">
		<!-- ! CARD -->
		<v-container class="mt-10 mt-xxl-16 primer-slide-container">
			<v-row class="d-flex justify-center">
				<v-card class="mb-6 px-6 mt-xxl-16 rounded-xl mx-2" elevation="0">
					<h1 class="px-2 py-4 text-orange-darken-2 text-xl-h2 text-h4 text-md-h2">
						Excelencia Digital, Adaptada para Ti
					</h1>
				</v-card>
			</v-row>
			<v-row class="mx-2 my-6 my-lg-16 v-flex align-center">
				<v-col cols="12" sm="5">
					<v-card
						class="mb-16 px-6 bg-orange-lighten-1 rounded-xl elementos-primera-pantalla"
						elevation="24"
					>
						<p
							class="px-2 py-4 text-md-h6 text-xl-h5 py-xl-16 px-xl-16 text-body-2 text-white typed-text"
						>
							{{ typedText }}
						</p>
					</v-card>
				</v-col>
				<v-col cols="2"></v-col>
				<v-col cols="5" v-if="$vuetify.display.smAndUp" class="mb-16 px-6 rotating-image">
					<v-img src="/css/pictures/service-title.png" cover class="elementos-primera-pantalla"></v-img>
				</v-col>
			</v-row>
		</v-container>
	</div>
		<div class="segunda-pantalla mb-16">
			<v-container> 
				<v-row>
					<!-- ! PRUEBA -->
					<v-col cols="12" sm="5" class="mt-16">
						<v-card
						class="mx-auto rounded-xl"
						max-width="700"
						elevation="24"
					  >
						<v-img
						  src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
						  height="400px"
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
					<v-col cols="2"></v-col>
					<v-col cols="12" sm="5" class="mt-16">
						<v-card
						class="mx-auto rounded-xl"
						max-width="700"
						elevation="24"
					  >

						<v-img
						  src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
						  height="400px"
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
					<v-col cols="12" sm="5" class="mt-16">
						<v-card
						class="mx-auto rounded-xl"
						max-width="700"
						elevation="24"
					  >

						<v-img
						  src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
						  height="400px"
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
					<v-col cols="2"></v-col>
					<v-col cols="12" sm="5" class="mt-16">
						<v-card
						class="mx-auto rounded-xl"
						max-width="700"
						elevation="24"
					  >

						<v-img
						  src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
						  height="400px"
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

					<v-col cols="12" sm="5" class="mt-16">
						<v-card
						class="mx-auto rounded-xl"
						max-width="700"
						elevation="24"
					  >

						<v-img
						  src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
						  height="400px"
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
					<v-col cols="2"></v-col>
					<v-col cols="12" sm="5" class="mt-16">
						<v-card
						class="mx-auto rounded-xl"
						max-width="700"
						elevation="24"
					  >

						<v-img
						  src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
						  height="400px"
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

					<v-col cols="12" sm="5" class="mt-16">
						<v-card
						class="mx-auto rounded-xl"
						max-width="700"
						elevation="24"
					  >

						<v-img
						  src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
						  height="400px"
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
					<v-col cols="2"></v-col>
					<v-col cols="12" sm="5" class="mt-16">
						<v-card
						class="mx-auto rounded-xl"
						max-width="700"
						elevation="24"
					  >

						<v-img
						  src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
						  height="400px"
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

					<!-- ! PRUEBA -->
				</v-row>
			</v-container>
		</div>
</div>	


</template>
<style>
.primera-pantalla {
	min-height: 100dvh;
}

.segunda-pantalla {
	min-height: 100dvh;
}

.toda-pagina {
	opacity: 0;
	animation: apareciendo 2s forwards;
}

.elementos-primera-pantalla {
	opacity: 0;
	animation: apareciendo 5s forwards 0.3s;
}

.rotating-image {
	animation: rotate 10s linear infinite; /* Adjust the duration as needed */
}

/* Optional: add styles for better readability or customization */
.typed-text::after {
	content: "|"; /* Cursor blink */
	animation: blink 0.7s infinite alternate;
}

@keyframes apareciendo {
	to {
		opacity: 1;
	}
}

@keyframes blink {
	to {
		opacity: 0;
	}
}

@keyframes rotate {
	from {
		transform: rotate(0deg);
	}
	to {
		transform: rotate(360deg);
	}
}
</style>
<script>
export default {
	data() {
		return {
			show: false,
			typedText: "",
			fullText:
				"Descubre una suite de servicios tecnológicos en EMPRESA diseñados para un impacto máximo. Desde el desarrollo de sitios web de vanguardia hasta integraciones de bases de datos sin fisuras y diseño web creativo, adaptamos soluciones para elevar tu marca. Nuestro marketing digital estratégico, aplicaciones web preparadas para el futuro y soluciones de comercio electrónico personalizadas redefinen el éxito en el panorama digital. Experimenta la innovación con EMPRESA, donde tu visión se encuentra con la excelencia digital.",
		};
	},
	methods: {
		typeText() {
			let index = 0;
			const intervalId = setInterval(() => {
				this.typedText = this.fullText.slice(0, index);
				index++;
				if (index > this.fullText.length) {
					clearInterval(intervalId);
				}
			}, 15);
		},
	},
	mounted() {
		this.typeText();
	},

	computed: {
		columnCount() {
			// Adjust the breakpoint as needed
			return this.$vuetify.display.smAndUp ? "6" : "12";
		},
	},
};
</script>
