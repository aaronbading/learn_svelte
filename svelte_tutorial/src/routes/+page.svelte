<script>
	import Nested from './Nested.svelte';
    import Button from './Button.svelte';
    import AddNumberButton from './AddNumberButton.svelte';
    import Info from './Info.svelte';

    const pkg = {
		name: 'svelte',
		version: 3,
		speed: 'blazing',
		website: 'https://svelte.dev'
	};


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
<Nested answer={42}/>
<Nested/> <!-- this is equivalent to the above line -->


<Button/>
<AddNumberButton/>


<!-- <Info name={pkg.name} version={pkg.version} speed={pkg.speed} website={pkg.website}/>  this is equivalent to the below line -->
<Info {...pkg}/>

