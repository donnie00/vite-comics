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
		<header class="d-flex justify-content-between">
			<a href="">
				<img class="nav-logo img-fluid" src="/img/dc-logo.png" alt="" />
			</a>
			<ul class="nav">
				<li v-for="link in navLinks" class="nav-item d-flex">
					<a
						class="nav-link text-uppercase d-flex align-items-center"
						href="#">
						{{ link }}
					</a>
				</li>
			</ul>
		</header>
	</div>
</template>

<style scoped lang="scss">
.nav-logo {
	// height: 100px;
	padding: 1rem 0;
}

.nav-link {
	font-size: 0.8rem;
	color: black;
	border-bottom: 3px solid transparent;

	&:hover {
		color: blue;
		border-bottom: 3px solid blue;
		background-color: rgba(0, 0, 255, 0.1);
	}
}
</style>
