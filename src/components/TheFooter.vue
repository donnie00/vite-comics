<script>
export default {
	data() {
		return {
			footerLinks: [
				{
					linkListName: 'Dc Comics',
					links: [
						{
							name: 'First link',
							href: '/',
						},
						{
							name: 'Second link',
							href: '/',
						},
						{
							name: 'Third link',
							href: '/',
						},
						{
							name: 'Fourth link',
							href: '/',
						},
						{
							name: 'Fifth link',
							href: '/',
						},
						{
							name: 'Sixth link',
							href: '/',
						},
						{
							name: 'Seventh link',
							href: '/',
						},
					],
				},
				{
					linkListName: 'Shop',
					links: [
						{
							name: 'First link',
							href: '/',
						},
						{
							name: 'Second link',
							href: '/',
						},
					],
				},
				{
					linkListName: 'DC',
					links: [
						{
							name: 'First link',
							href: '/',
						},
						{
							name: 'Second link',
							href: '/',
						},
						{
							name: 'Third link',
							href: '/',
						},
						{
							name: 'Fourth link',
							href: '/',
						},
						{
							name: 'Fifth link',
							href: '/',
						},
						{
							name: 'Sixth link',
							href: '/',
						},
						{
							name: 'Seventh link',
							href: '/',
						},
						{
							name: 'Seventh link',
							href: '/',
						},
						{
							name: 'Seventh link',
							href: '/',
						},
						{
							name: 'Seventh link',
							href: '/',
						},
						{
							name: 'Seventh link',
							href: '/',
						},
					],
				},
				{
					linkListName: 'Sites',
					links: [
						{
							name: 'First link',
							href: '/',
						},
						{
							name: 'Second link',
							href: '/',
						},
						{
							name: 'Third link',
							href: '/',
						},
						{
							name: 'Fourth link',
							href: '/',
						},
						{
							name: 'Fifth link',
							href: '/',
						},
					],
				},
			],
		};
	},
};
</script>

<template>
	<div class="bg-heroes-img">
		<div class="container">
			<div class="row">
				<div class="col-7 py-5">
					<div class="d-flex align-items-baseline">
						<div
							v-for="(linkList, i) in footerLinks"
							class="list-wrapper">
							<h5 class="text-uppercase">{{ linkList.linkListName }}</h5>
							<ul class="list-unstyled">
								<li v-for="link in linkList.links" class="list-item">
									<a :href="link.href"> {{ link.name }} </a>
								</li>
							</ul>
						</div>
					</div>
				</div>
				<div class="col bg-logo"></div>
			</div>
		</div>
	</div>
</template>

<style lang="scss" scoped>
.bg-heroes-img {
	background-image: url(/img/footer-bg.jpg);
	background-repeat: no-repeat;
	background-size: cover;
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
