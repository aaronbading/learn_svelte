<script>
	import Nested from './Nested.svelte';
    import Button from './Button.svelte';
    let name = 'world';
    let src = 'https://media.giphy.com/media/3o7aD2jBmUohFAOZ5W/giphy.gif';
    // let src = '../../static/favicon.png';  // dont know why this does not work .. 

    
</script>

<style>
    p {
    color: purple;
    font-family: 'Comic Sans MS', cursive;
    font-size: 2em;
}
</style>

<h1>Hello {name}!</h1>
<img {src} alt="A man dances.">
<Nested />

<Button/>

