<script>
	import Map from './Map.svelte';
	import Search from './Search.svelte';
	export let ready;
</script>

<svelte:head>
	<script defer async
	src="https://maps.googleapis.com/maps/api/js?key=AIzaSyB1uyREZS2OOcs48tRnhmTyqt0K0E078-U&callback=initMap">
	</script>
</svelte:head>

<style>
:global(body) {
	padding: 0;
}
</style>

{ #if ready }
<Search></Search>
<Map></Map>
{ /if }