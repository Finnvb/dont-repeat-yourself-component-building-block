<script>
	export let inputName;
	export let placeholder;
</script>

<input type="text" id={inputName} {placeholder} required />

<style>
	input {
		width: 80%;
		height: 2rem;
		border: none;
		font-size: 0.8rem;
	}
</style>
