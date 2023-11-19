<!-- ! TEMPLATE -->

<template>
	<div class="main-div">
		<v-carousel
			:continuous="true"
			hide-delimiter-background
			height="100vh"
			cycle
			show-arrows="hover"
		>
			<v-carousel-item
				v-for="(slide, i) in slides"
				:key="i"
				:src="slide.image"
				cover
			>
				<div class="heading-carousel">
					<h1 class="heading-carousel-title">{{ slide.title }}</h1>
					<p class="heading-carousel-subtitle">{{ slide.subtitle }}</p>
				</div>
			</v-carousel-item>
		</v-carousel>
	</div>
	<!-- ? Here I will insert a component which is in another folder, in order to provide path I should do <folder>-<component> -->
	<extra-Cookies />
	<mainPage-secondScreen />

</template>

<!-- ! STYLE -->

<style>
.main-div {
	top: 5rem;
}

.heading-carousel {
	position: relative;
	left: 10rem;
	margin-right: 2rem;
	color: white;
	top: 20%;
	padding: 0.5rem;
}

.heading-carousel-title {
	position: relative;
	width: 60%;
	min-width: 35rem;
	font-size: 4rem;
	font-weight: bold;
	padding: 0.5rem;
	background-color: rgba(255, 128, 0, 0.514);
	opacity: 0;
	animation: tituloApareciendo 3s forwards;
}

.heading-carousel-subtitle {
	position: relative;
	font-size: 2rem;
	margin-top: 1rem;
	width: fit-content;
	max-width: 80%;
	padding: 0.5rem;
	background-color: rgba(241, 241, 241, 0.627);
	color: rgb(66, 66, 66);
	opacity: 0;
	animation: subtituloApareciendo 1s forwards 3s;
}

/* Animations */

@keyframes tituloApareciendo {
	20% {
		opacity: 0;
	}
	80% {
		transform: scale(1.1);
	}
	100% {
		opacity: 1;
	}
}

@keyframes subtituloApareciendo {
	from {
		opacity: 0;
	}
	to {
		opacity: 1;
	}
}

/* Screen sizes */

@media screen and (max-width: 680px) {
	.heading-carousel {
		top: 10%;
		width: fit-content;
	}

	.heading-carousel-title {
		width: fit-content;
		min-width: auto;
		padding: 5rem 2rem;
		height: 20rem;
		font-size: 1.6rem;
	}
	.heading-carousel-subtitle {
		margin-top: 2rem;
		font-size: 1.15rem;
	}

	.heading-carousel {
		margin: 10%;
		left: 0rem;
	}
}


</style>

<!-- ! TYPESCRIPT -->

<script>
export default {
	data() {
		return {
			slides: [
				{
					image: "/css/pictures/carousel-1.jpg",
					title: "Soluciones Tecnológicas para el Éxito Empresarial",
					subtitle: "Mejora tu Rendimiento con Estrategias a la Medida",
				},
				{
					image: "/css/pictures/carousel-2.jpg",
					title: "Posicionamiento Estratégico en la Web",
					subtitle: "Optimice su Visibilidad y Aumente su Alcance en la Web",
				},
				{
					image: "/css/pictures/carousel-3.jpg",
					title: "Bases de Datos Potentes para su Negocio",
					subtitle:
						"Optimice el Manejo de Datos para Decisiones Más Inteligentes y Rápidas",
				},
			],
			headings: ["hey", "hello"],
		};
	},
};
</script>
