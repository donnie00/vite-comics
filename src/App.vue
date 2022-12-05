<script>
import TheHeader from './components/TheHeader.vue';
import BuyComicsBanner from './components/BuyComicsBanner.vue';
import TheFooter from './components/TheFooter.vue';
import ContactsBanner from './components/ContactsBanner.vue';
import Jumbotron from './components/Jumbotron.vue';
import Card from './components/Card.vue';

import comicsData from './composables/comicsData.js';

export default {
	components: {
		TheHeader,
		TheFooter,
		BuyComicsBanner,
		ContactsBanner,
		Jumbotron,
		Card,
	},

	data() {
		return {
			comicsData,
		};
	},
};
</script>

<template>
	<TheHeader />
	<Jumbotron />
	<main class="bg-dark pb-2">
		<div class="container comics-container">
			<h5 class="text-white bg-primary d-inline-block p-2">
				Current Series
			</h5>

			<div class="row row-cols-6 g-3 p-2">
				<Card
					v-for="(singleComic, i) in comicsData"
					:key="'comic_' + i"
					:comic="singleComic" />
			</div>
			<button
				class="btn btn-primary text-light text-uppercase rounded-0 d-block mx-auto">
				Load more
			</button>
		</div>
	</main>

	<BuyComicsBanner />
	<TheFooter />
	<ContactsBanner />
</template>

<style lang="scss">
@use './styles/partials/variables' as *;

main {
	h5 {
		margin-top: -20px;
	}
	.comics-container {
		button {
			padding-inline: 3rem;
			background-color: $main-color;
		}
	}
}
</style>
