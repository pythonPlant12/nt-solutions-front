<template>
	<header class="border-gray-400">
		<!-- ! Navigation Bar MOBILE-->
		<div class="container">
			<nav class="nav">
				<ul class="nav-list nav-list-mobile">
					<li class="nav-item">
						<div class="mobile-menu">
							<span class="line line-top"></span>
							<span class="line line-buttom"></span>
							<span class="line line-buttom1"></span>
						</div>
					</li>
					<li class="nav-item">
						<nuxt-link to="/" class="nav-link nav-link-apple"></nuxt-link>
					</li>
					<li class="nav-item">
						<a href="#" class="nav-link nav-link-bag"></a>
					</li>
				</ul>
				<!-- /.nav-list nav-list-mobile -->
				<!-- ! Navigation List of Options Bar COMPUTER -->
				<ul class="nav-list nav-list-larger larger-mobile">
					<li class="nav-item nav-item-hidden">
						<div class="mobile-menu">
							<span class="line line-top"></span>
							<span class="line line-bottom"></span>
						</div>
					</li>
					<li class="nav-item">
						<a href="#" class="nav-link"></a>
					</li>

					<li class="nav-item">
						<nuxt-link to="/" class="nav-link nav-link-mobile" @click.prevent="cerrarMenu()"
							><v-btn :color="empresa" append-icon="mdi mdi-domain" size="large" variant="text"
								>Empresa</v-btn
							></nuxt-link
						>
					</li>
					<li class="nav-item">
						<nuxt-link
							to="/servicios"
							class="nav-link nav-link-mobile"
							@click.prevent="cerrarMenu()"
							><v-btn
								:color="servicios"
								append-icon="mdi mdi-database-cog"
								size="large"
								variant="text"
								>Servicios</v-btn
							></nuxt-link
						>
					</li>
					<li class="nav-item">
						<nuxt-link
							to="/tecnologias"
							class="nav-link nav-link-mobile"
							@click.prevent="cerrarMenu()"
							><v-btn
								:color="tecnologias"
								append-icon="mdi mdi-wifi-settings"
								size="large"
								variant="text"
								>Tecnologías</v-btn
							></nuxt-link
						>
					</li>
					<li class="nav-item">
						<nuxt-link
							to="/sobre-nosotros"
							class="nav-link nav-link-mobile"
							@click.prevent="cerrarMenu()"
							><v-btn
								:color="sobreNosotros"
								append-icon="mdi mdi-information-variant"
								size="large"
								variant="text"
								>Sobre Nosotros</v-btn
							></nuxt-link
						>
					</li>
					<li class="nav-item">
						<nuxt-link to="/contacto" class="nav-link nav-link-mobile" @click.prevent="cerrarMenu()"
							><v-btn
								:color="contacto"
								append-icon="mdi mdi-account-box-outline"
								variant="text"
								size="large"
								>Contacto</v-btn
							>
						</nuxt-link>
					</li>
				</ul>
			</nav>
		</div>
	</header>
	<div class="mt-16">
		<slot />
		<extra-Cookies @aceptarCookies="updateCookieData" v-if="cookiesAceptadas"/>
	</div>
	<footer>
		<div class="footer footer-main">
			<div class="footer footer-div">
				<v-btn v-for="icon in icons" :key="icon" class="mx-4" :icon="icon" variant="text"></v-btn>
			</div>
			<div class="footer footer-div">
				<p>
					Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laudantium vitae fuga veniam,
					delectus minus facilis veritatis ipsum nisi quibusdam, molestias pariatur illo facere
					dolorem dignissimos beatae libero odio tenetur totam! Temporibus atque consequuntur
					quaerat vitae ab eligendi cumque quos ipsa doloribus, aperiam quis at placeat et harum
					nisi vero odit incidunt numquam dolor, autem maxime possimus mollitia deleniti non. Ipsum
					odio corporis a veniam vel dolor, pariatur ex quia commodi consectetur illum quod fugit
					ducimus deserunt officia quam quae nihil voluptas aut distinctio rem, sed harum unde?
					Cumque quibusdam sequi atque distinctio. Ullam ratione eligendi ipsa asperiores voluptate
					repudiandae numquam explicabo beatae iusto incidunt sint, dolorum voluptatibus. Hic
					aliquid consequuntur iste ab, obcaecati, molestiae doloremque laborum quidem error vitae,
					accusamus facere porro at eos quas eum et inventore repudiandae reprehenderit pariatur.
					Corporis, dolorum voluptatem incidunt quas ut accusamus magnam magni rerum illum
					cupiditate laboriosam repudiandae aliquid, neque architecto enim? Aliquid quibusdam dicta
					nisi temporibus quisquam facere cumque aspernatur eos quis. Asperiores molestiae nam
					commodi minus aliquam dolore sunt, ex numquam ipsa harum nisi aspernatur, perferendis qui
					enim veniam, officia delectus ad consectetur quos excepturi cum sint. Reprehenderit minus
					temporibus, expedita id accusamus vero sapiente a aliquid natus qui eligendi et.
				</p>
			</div>
		</div>
	</footer>
</template>

<style>
a {
	display: block;
	text-decoration: none;
}
/* ! Header */
header {
	display: flex; /* Use flexbox */
	justify-content: center; /* Center horizontally */
	align-items: center; /* Center vertically */
	position: fixed;
	top: 0;
	z-index: 14;
	width: 100%;
	height: 4.4rem;
	background-color: rgba(248, 248, 248, 0.5);
	backdrop-filter: blur(2rem);
	border-bottom-width: 1px;
}

.nav-list {
	list-style: none;
	display: flex;
	align-items: center;
	justify-content: space-between;
	margin: 0 -1rem;
}

.nav-list-mobile {
	display: none;
}

.nav-link {
	font-size: 1.4rem;
	color: #5f5a5a;
	width: 100%;
	padding: 0 1rem;
	transition: opacity 0.5s;
}
.nav-link:hover {
	opacity: 0.7;
}

.nav-link-apple {
	align-self: center;
	width: 1.6rem;
	height: 4.4rem;
	background: url("~/css/icons/apple.svg") center no-repeat;
}

.nav-link-search {
	width: 1.6rem;
	height: 4.4rem;
	background: url("~/css/icons/search.svg") center no-repeat;
}

.nav-link-bag {
	margin-right: 2rem;
	align-self: center;
	width: 1.4rem;
	height: 4.4rem;
	background: url("~/css/icons/bag.svg") center no-repeat;
}

@media screen and (max-width: 1100px) {
	.hero {
		height: 100rem;
		background-size: auto 100rem;
		background-position: bottom center;
		background-repeat: no-repeat;
	}

	header {
		display: block; /* Use flexbox */
	}
	.title-heading {
		font-size: 4.4rem;
	}

	.title-sub-heading {
		font-size: 2.4rem;
		color: white;
	}

	.cta-link:nth-child(2) {
		margin-left: 2rem;
	}

	.title-heading-watch {
		height: 6.2rem;
		/* background-image: url("images/hero/watch/logo_watch_medium.png"); */
		background-size: auto 6.2rem;
	}
}

/* ! CSS Styles for PHONE (Small Screen ) */
@media screen and (max-width: 1100px) {
	header {
		height: 4.8rem;
		transition: background 0.36s cubic-bezier(0.32, 0.08, 0.24, 1),
			height 0.5s cubic-bezier(0.32, 0.08, 0.24, 1);
	}

	header .container {
		padding: 0;
	}

	.iphone-11-pro {
		margin-top: 4.8rem;
	}

	.nav-list {
		margin-top: 0;
	}

	.nav-list-mobile {
		display: flex;
	}

	.nav-item {
		width: 4.8rem;
		height: 4.8rem;
		display: flex;
		justify-content: center;
	}

	.nav-link-mobile {
		padding-bottom: 8px;
		border-bottom-width: 2px;
		border-color: #2a2a2a10;
	}

	.nav-item-hidden {
		display: none;
	}

	/* ! Lines of mobile menu trigger */
	.mobile-menu {
		margin-left: 2rem;
		position: relative;
		z-index: 15;
		width: 100%;
		height: 100%;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		cursor: pointer;
	}

	.line {
		position: absolute;
		width: 1.7rem;
		height: 1.4px;
		background-color: #413f3f;
		color: #413f3f;
		transition: margin-top 0.3192s cubic-bezier(0.04, 0.04, 0.12, 0.96);
	}

	.line-top {
		transform: translateX(10px);
		transform: rotate(0deg);
		transition: transform 0.3192s 0.1s cubic-bezier(0.04, 0.04, 0.12, 0.96);
	}
	.line-buttom {
		margin-top: -0.4px;
		transform: rotate(0deg);
		transition: transform 0.3192s 0.1s cubic-bezier(0.04, 0.04, 0.12, 0.96);
	}

	.line-buttom1 {
		margin-top: 10px;
		opacity: 1;
		transition: margin-top 0.3192s 0.1s cubic-bezier(0.04, 0.04, 0.12, 0.96);
		transition: opacity 0.3192s 0.2s cubic-bezier(0.04, 0.04, 0.12, 0.96);
		transition-delay: 0.1s;
	}

	.active .line-buttom1 {
		margin-top: 0px;
		opacity: 0;
		transition-delay: 0.1s;
		transition: margin-top 0.3192s 0.1s cubic-bezier(0.04, 0.04, 0.12, 0.96);
	}
	/* ! Mobile Menu Trigger transition/transform */

	.active .line-top {
		margin-bottom: 0;
		transform: rotate(45deg);
		transition: transform 0.3192s 0.1s cubic-bezier(0.04, 0.04, 0.12, 0.96);
	}
	.active .line-buttom {
		margin-top: 0;
		transform: rotate(-45deg);
		transition: transform 0.3192s 0.1s cubic-bezier(0.04, 0.04, 0.12, 0.96);
	}

	header.active {
		height: 100%;
		background-color: rgba(244, 239, 239, 1);
		backdrop-filter: blur(1rem);
	}

	.nav-link-apple {
		width: 1.8rem;
		height: 4.8rem;
		position: relative;
		z-index: 15;
	}

	.nav-link-bag {
		width: 1.6rem;
		height: 4.8rem;
		transition: opacity 3s;
	}

	.nav {
		position: relative;
	}

	.nav-link {
		font-size: 1.7rem;
		padding: 0;
		margin: auto 0;
	}

	.nav-list-larger {
		position: fixed;
		opacity: 0;
		/* ! */
		visibility: hidden;
		top: 0;
		left: 0;
		width: 0;
		height: 0;
		display: block;
		padding: 10.5rem 5rem;
		z-index: 10;
		box-sizing: border-box;
		transition: opacity 0.3s;
	}

	.active .nav-link-bag {
		opacity: 0;
		transition: opacity 0.3s;
	}

	.nav-list-larger .nav-item {
		width: 100%;
		justify-content: flex-start;
		border-bottom: 4px solid rgba(255, 255, 255, 0.1);
	}
	.nav-list-larger .nav-item:nth-child(9) {
		border-bottom: none;
	}
}
.active .nav-list-larger .nav-item {
	opacity: 1;
}
.active .nav-list-larger {
	animation: fadeIn 1s ease-in;
	opacity: 1;
	width: 100%;
	height: 100vh;
	visibility: visible;
}
@keyframes fadeIn {
	from {
		opacity: 0;
		visibility: hidden;
	}
	to {
		opacity: 1;
		visibility: visible;
	}
}

.footer {
	display: flex;
}

.footer-main {
	border-top: 1px;
	border-top-style: solid;
	border-color: gray;
	flex-direction: column;
}

.footer-div {
	margin-top: 1rem;
	justify-content: center;
}

.main-div {
	height: 100dvh;
}
</style>
<script>
export default {
	mounted() {
		this.cookiesAceptadas = true;
		const selectElement = (element) => document.querySelector(element);

		selectElement(".mobile-menu").addEventListener("click", () => {
			selectElement("header").classList.toggle("active");
		});
	},
	data() {
		return {
			icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
			cookiesAceptadas: false
		};
	},
	methods: {
		cerrarMenu() {
			const selectElement = (element) => document.querySelector(element);
			selectElement("header").classList.remove("active");
		},
		updateCookieData() {
      		this.cookiesAceptadas = true;
    },
	},

	computed: {
		empresa() {
			const currentPath = this.$route.path;
			if (currentPath === "/") {
				return "orange";
			}
		},
		servicios() {
			const currentPath = this.$route.path;
			if (currentPath === "/servicios") {
				return "orange";
			}
		},
		tecnologias() {
			const currentPath = this.$route.path;
			if (currentPath === "/tecnologias") {
				return "orange";
			}
		},
		sobreNosotros() {
			const currentPath = this.$route.path;
			if (currentPath === "/sobre-nosotros") {
				return "orange";
			}
		},
		contacto() {
			const currentPath = this.$route.path;
			if (currentPath === "/contacto") {
				return "orange";
			}
		},
	},
};
</script>
