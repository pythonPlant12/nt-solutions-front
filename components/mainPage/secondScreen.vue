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
			<h2 class="titulo text-h2 font-weight-black text-orange">Empresa en un mundo digital</h2>

			<div class="subtitulo text-h4 font-weight-medium mb-8 mt-8">Si estás aqui es porque...</div>

			<p class="texto text-h6 mb-8 mt-8">
				valoras la excelencia en la presencia digital de tu negocio. En nuestra plataforma, te
				ofrecemos no solo servicios de diseño web vanguardistas, sino también soluciones
				tecnológicas personalizadas para potenciar el rendimiento de tu empresa. Desde la
				implementación de bases de datos hasta la creación de portales especializados, nuestro
				compromiso es impulsar tu éxito en línea. Con enfoque en el posicionamiento web y SEO, nos
				esforzamos por llevar tu presencia digital a nuevas alturas. ¡Descubre cómo podemos
				transformar tu visión en una realidad digital impactante y efectiva!
			</p>

			<nuxt-link to="/servicios"
				><v-btn color="orange" size="x-large" elevation="4">Descubrir</v-btn></nuxt-link
			>
		</div>
	</v-sheet>

	<v-sheet
		class=""
		elevation="4"
		height="100vh"
		rounded
    min-width="80%"
		width="100%"
	>
		<h1 class="text-sm-h2 py-sm-16 py-8 font-weight-black text-orange px-8">
			Preguntas más frecuentes...
		</h1>

		<template>
			<v-expansion-panels variant="popout" class="pa-sm-4 px-0">
				<v-expansion-panel v-for="(message, i) in messages" :key="i" hide-actions>
					<v-expansion-panel-title>
						<v-row align="center" class="spacer" no-gutters>
							<v-col class="text-no-wrap text-left" cols="5" sm="3">
								<v-chip
									v-if="message.tag"
									:color="`${message.color}-lighten-1`"
									class="ms-0 me-2"
									label
									small
								>
									{{ message.tag }}
								</v-chip>
								<strong>{{ message.title }}</strong>
							</v-col>

							<v-col
								v-if="message.excerpt"
								class="text-medium-emphasis text-truncate hidden-sm-and-down"
							>
								&mdash;
								{{ message.excerpt }}
							</v-col>
						</v-row>
					</v-expansion-panel-title>

					<v-expansion-panel-text>
						<h3 class="text-h6">{{ message.excerpt }}</h3>
						<v-card-text v-text="message.text"></v-card-text>
					</v-expansion-panel-text>
				</v-expansion-panel>
			</v-expansion-panels>
		</template>
	</v-sheet>
</template>

<style>
.sheet {
  opacity: 1 !important;
  z-index: 10 !important
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
		messages: [
			{
				avatar: "https://avatars0.githubusercontent.com/u/9064066?v=4&s=460",
				name: "John Leider",
				title: "Desarrollo Web Personalizado",
        color: "orange",
				excerpt:
					"¿Cómo beneficia un desarrollo web personalizado a mi empresa?",
        text: "El desarrollo web personalizado ofrece soluciones adaptadas a las necesidades específicas, proporcionando flexibilidad y eficacia para un sitio web único.",
        tag: 1
			},
			{
				icon: "mdi-account-multiple",
				name: "Servicios Especializados",
        excerpt:"¿Cuáles son las ventajas de elegir servicios especializados?",
				tag: 2,
				total: 3,
				title: "Servicios Especializados",
        text: "Optar por servicios especializados garantiza un enfoque centrado en las necesidades únicas de tu empresa, brindando soluciones más adaptadas que las plataformas estándar."
			},
			{
				icon: "mdi-tag",
				name: "Promos",
        color: "orange",
				tag: 3,
				total: 4,
				title: "SEO Personalizado",
				excerpt: "¿Ofrecen servicios de SEO personalizados para mejorar la visibilidad?",
        text: "Sí, la integración de estrategias de SEO personalizadas aumenta la visibilidad del sitio web, mejorando el ranking en los motores de búsqueda y atrayendo más tráfico orgánico."
			},
      {
				icon: "mdi-tag",
				name: "Promos",
				tag: 4,
				total: 4,
				title: "Comercio Electrónico Adaptable",
				excerpt: "¿Pueden incorporar funcionalidades de comercio electrónico específicas?",
        text: "Absolutamente, el desarrollo personalizado permite la integración de soluciones de comercio electrónico adaptadas a las necesidades específicas de tu empresa."
			},
      {
        color: "orange",
				icon: "mdi-tag",
				name: "Promos",
				tag: 5,
				total: 4,
				title: "Promoción Digital Integral",
				excerpt: "¿Cómo se promocionan los sitios web empresariales desarrollados?",
        text: "Empleamos estrategias de marketing digital integral, incluyendo redes sociales, contenido atractivo y publicidad en línea, para aumentar la visibilidad de los servicios en línea."
			},
		],
		lorem:
			"Lorem ipsum dolor sit amet, at aliquam vivendum vel, everti delicatissimi cu eos. Dico iuvaret debitis mel an, et cum zril menandri. Eum in consul legimus accusam. Ea dico abhorreant duo, quo illum minimum incorrupte no, nostro voluptaria sea eu. Suas eligendi ius at, at nemore equidem est. Sed in error hendrerit, in consul constituam cum.",
	}),
};
</script>
