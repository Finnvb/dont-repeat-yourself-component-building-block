<script>
	export let imgSource;
</script>

<img src={imgSource} alt="formImg" />

<style>
	img {
		width: 15rem;
		height: 100%;
		padding-right: 2rem;
	}

	@media (max-width: 40rem) {
		img {
			display: none;
		}
	}
</style>
