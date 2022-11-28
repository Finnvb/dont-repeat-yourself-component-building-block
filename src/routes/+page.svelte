<script>
	import Title from '$lib/components/Title.svelte';
	import Label from '$lib/components/Label.svelte';
	import Input from '$lib/components/Input.svelte';
	import Button from '../lib/components/Button.svelte';
	import Textarea from '../lib/components/Textarea.svelte';
	import Image from '../lib/components/Image.svelte';
	import '../styles/global.css';
</script>

<svelte:head>
	<title>Ilojo Bar - Form Component</title>
</svelte:head>

<section>
	<form>
		<Title />
		<Label labelName="name" labelText="Name" />
		<Input inputName="name" placeholder="John Doe" />
		<Label labelName="email" labelText="Your email" />
		<Input inputName="email" placeholder="johndoe@mail.com" />
		<Label labelName="storytitle" labelText="Storytitle" />
		<Input inputName="storytitle" placeholder="Awesome story!" />
		<Label labelName="content" labelText="Content" />
		<Textarea placeholder="Lorem ipsum" />
		<Button btnText="Send Story" />
	</form>
	<Image imgSource="/book-stand.png" />
</section>

<style>
	form {
		width: 25rem;
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		gap: 1rem;
		background-color: #8c0500;
		margin-right: 2rem;
	}

	section {
		display: inline-flex;
		flex-direction: row;
		align-items: center;
		background-color: #8c0500;
		padding: 1rem 0;
	}

	@media (max-width: 40rem) {
		form {
			/* width: 15rem; */
			gap: 0.2em;
			margin-right: 0rem;
		}
	}
</style>
