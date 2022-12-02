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
			<img class="navbar-brand img-fluid" src="/img/dc-logo.png" alt="" />
			<ul class="nav">
				<li v-for="link in navLinks" class="nav-item">
					<a class="nav-link link-dark text-uppercase" href="#">
						{{ link }}
					</a>
				</li>
			</ul>
		</header>
	</div>
</template>
