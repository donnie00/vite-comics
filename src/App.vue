<script>
import TheHeader from './components/TheHeader.vue';
import buyComicsBanner from './components/buyComicsBanner.vue';
import TheFooter from './components/TheFooter.vue';
export default {
	components: {TheHeader, buyComicsBanner, TheFooter},
};
</script>

<template>
	<TheHeader></TheHeader>
	<main class="bg-dark py-5">
		<div class="container">
			<h3 class="text-light">Main content here</h3>
		</div>
	</main>
	<buyComicsBanner></buyComicsBanner>
	<TheFooter></TheFooter>
</template>

<style></style>
