<script>
	import Map from './Map.svelte';
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
<Map></Map>
{ /if }