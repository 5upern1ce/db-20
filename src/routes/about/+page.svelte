<script>
	import Navbar from '$lib/Navbar.svelte';
	import Carousel from '$lib/Carousel.svelte';
</script>

<Navbar />
<div class="bg-red-500">
	<!-- full width row, center the inner fixed-width box -->
	<div class="flex w-full justify-center pt-3">
		<div class="w-[800px] max-w-full">
			<!-- change 800px or use max-w-4xl -->
			<Carousel />
		</div>
	</div>
</div>
