<script>
export default {
	data() {
		return {};
	},
};
</script>

<template>
	<div class="bg-heroes-img">
		<div class="container">
			<div class="row">
				<div class="col-7 py-5">
					<div class="d-flex">
						<div class="list-wrapper">
							<h5 class="text-uppercase">Dc comics</h5>
							<ul class="list-unstyled">
								<li class="list-item">
									<a href=""> An item </a>
								</li>
								<li class="list-item">
									<a href=""> A second item </a>
								</li>
								<li class="list-item">
									<a href=""> A third item </a>
								</li>
								<li class="list-item">
									<a href=""> A fourth item </a>
								</li>
								<li class="list-item">
									<a href=""> And a fifth one </a>
								</li>
							</ul>

							<h5 class="text-uppercase">Shop</h5>
							<ul class="list-unstyled">
								<li class="list-item">
									<a href=""> An item </a>
								</li>
								<li class="list-item">
									<a href=""> A second item </a>
								</li>
							</ul>
						</div>

						<div class="list-wrapper">
							<h5 class="text-uppercase">DC</h5>
							<ul class="list-unstyled">
								<li class="list-item">
									<a href=""> An item </a>
								</li>
								<li class="list-item">
									<a href=""> A second item </a>
								</li>
								<li class="list-item">
									<a href=""> A third item </a>
								</li>
								<li class="list-item">
									<a href=""> A fourth item </a>
								</li>
								<li class="list-item">
									<a href=""> And a fifth one </a>
								</li>
								<li class="list-item">
									<a href=""> And a fifth one </a>
								</li>
								<li class="list-item">
									<a href=""> And a fifth one </a>
								</li>
								<li class="list-item">
									<a href=""> And a fifth one </a>
								</li>
								<li class="list-item">
									<a href=""> And a fifth one </a>
								</li>
							</ul>
						</div>

						<div class="list-wrapper">
							<h5 class="text-uppercase">Sites</h5>
							<ul class="list-unstyled">
								<li class="list-item">
									<a href=""> An item </a>
								</li>
								<li class="list-item">
									<a href=""> A second item </a>
								</li>
								<li class="list-item">
									<a href=""> A third item </a>
								</li>
								<li class="list-item">
									<a href=""> A fourth item </a>
								</li>
								<li class="list-item">
									<a href=""> And a fifth one </a>
								</li>
							</ul>
						</div>
					</div>
				</div>
				<div class="col-5 bg-logo"></div>
			</div>
		</div>
	</div>
</template>

<style lang="scss" scoped>
.bg-heroes-img {
	background-image: url(/img/footer-bg.jpg);
}
.bg-logo {
	background-image: url(/img/dc-logo-bg.png);
	background-position: center;
	background-size: cover;
}

.list-wrapper {
	padding-right: 1rem;

	h5 {
		color: white;
	}

	a {
		color: grey;
		text-decoration: none;

		&:hover {
			opacity: 0.8;
		}
	}
}
</style>
