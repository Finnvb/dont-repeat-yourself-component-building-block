<script>
	import Title from '$lib/components/Title.svelte';
	import Label from '$lib/components/Label.svelte';
    import Input from '$lib/components/Input.svelte';
    import Button from '../lib/components/Button.svelte';
    import Textarea from '../lib/components/Textarea.svelte';
    import '../styles/global.css'
</script>

<form>
<Title/>
<Label labelName='name' labelText='Name'/>
<Input inputName='name' placeholder='John Doe'/>
<Label labelName='email' labelText='Your email'/>
<Input inputName='email' placeholder='johndoe@mail.com'/>
<Label labelName='storytitle' labelText='Storytitle'/>
<Input inputName='storytitle' placeholder='Awesome story'/>
<Label labelName='content' labelText='Content'/>
<Textarea placeholder='Lorem ipsum'/>
<Button btnText='Send Story'/>
</form>


<style>

    form{
        width: 25rem;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background-color: #8C0500;
    }
</style>