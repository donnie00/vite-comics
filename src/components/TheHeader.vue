<script>
export default {
	data() {
		return {
			navLinks: [
				'characters',
				'comics',
				'movies',
				'tv',
				'games',
				'collectibles',
				'video',
				'fans',
				'news',
				'shop',
			],
		};
	},
};
</script>

<template>
	<div class="container">
		<header class="navbar">
			<img class="navbar-brand" src="/img/dc-logo.png" alt="" />
			<ul class="nav">
				<li v-for="link in navLinks" class="nav-item">
					<a class="nav-link link-dark" href="#">
						<!-- Da cambiare con sass css in uppercase -->
						{{ link.toUpperCase() }}
					</a>
				</li>
			</ul>
		</header>
	</div>
</template>
