<script>
export default {
	data() {
		return {
			sectionsLinks: [
				{
					name: 'digital comics',
					icon: 'buy-comics-digital-comics.png',
				},
				{
					name: 'dc merchandise',
					icon: 'buy-comics-merchandise.png',
				},
				{
					name: 'subsription',
					icon: 'buy-comics-subscriptions.png',
				},
				{
					name: 'comic shop locator',
					icon: 'buy-comics-shop-locator.png',
				},
				{
					name: 'dc power visa',
					icon: 'buy-dc-power-visa.svg',
				},
			],
		};
	},
};
</script>

<template>
	<div class="bg-primary py-5">
		<div class="container">
			<ul class="nav align-items-center justify-content-center">
				<li
					class="nav-item align-items-center"
					v-for="section in sectionsLinks">
					<a class="nav-link link-light" href="">
						<img class="img-fluid" :src="`/img/${section.icon}`" alt="" />
						<span class="text-uppercase">{{ section.name }}</span>
					</a>
				</li>
			</ul>
		</div>
	</div>
</template>
