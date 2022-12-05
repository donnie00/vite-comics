<script>
export default {
	props: {
		comic: {
			type: Object,
			required: true,
		},
	},

	data() {
		return {};
	},
};
</script>

<template>
	<div class="col">
		<div class="my-card">
			<div class="card-body">
				<img class="img-fluid" :src="comic.thumb" alt="" />
				<p class="card-label">{{ comic.series }}</p>
			</div>
		</div>
	</div>
</template>
<style lang="scss">
@use '../styles/partials/variables' as *;
.my-card {
	transition: all 0.1s linear;

	.card-body {
		img {
			aspect-ratio: 1/1;
			object-fit: cover;
			object-position: top;
			margin-bottom: 0.5rem;
		}

		.card-label {
			font-size: 0.7rem;
			color: white;
			text-transform: uppercase;
		}
	}

	&:hover {
		scale: 1.1;
		font-weight: bold;

		.card-label {
			color: $main-color;
		}
	}
}
</style>
