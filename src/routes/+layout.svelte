<!-- This +layout page sets a default layout across pages -->
<script lang="ts">
	import '../app.css';
	import favicon from '$lib/assets/favicon.svg';
	import Navbar from '$lib/Navbar.svelte';
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<meta name="viewport" content="width=device-width, user-scalable=no" />
</svelte:head>

<!-- <Navbar /> is a self closing element that calls the navbar element from Navbar.svelte -->
<Navbar />
{@render children?.()}
