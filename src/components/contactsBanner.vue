<script>
export default {
	data() {
		return {
			socialLinks: [
				'facebook',
				'twitter',
				'youtube',
				'pinterest',
				'periscope',
			],
		};
	},
};
</script>

<template>
	<div class="py-4 my-bg-secondary">
		<div class="container">
			<div class="d-flex align-items-center">
				<button
					class="btn btn-outline-primary rounded-0 text-uppercase text-light">
					Sign-up now!
				</button>

				<div class="link-container d-flex align-items-center gap-3 ms-auto">
					<h5 class="text-primary text-uppercase fw-bold m-0">
						Follow us
					</h5>
					<ul class="list-unstyled list-inline m-0">
						<li v-for="social in socialLinks" class="list-inline-item">
							<a href="#">
								<img
									class="px-1"
									:src="`/img/footer-${social}.png`"
									alt="" />
							</a>
						</li>
					</ul>
				</div>
			</div>
		</div>
	</div>
</template>

<style scoped>
.my-bg-secondary {
	background-color: #303030;
}
</style>
