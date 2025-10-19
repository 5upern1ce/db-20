<script lang="ts">
	import { Carousel, Controls, CarouselIndicators } from 'flowbite-svelte';
	import type { HTMLImgAttributes } from 'svelte/elements';

	const { images } = $props();

	let index = $state(0);
	let image: HTMLImgAttributes | undefined = $state();
</script>

<div class=" max-w-6xl space-y-4">
	<!-- 'onchange={(detail)}' sets the text under the image to the current alt of the image -->
	<!-- 'duration' is measured in milliseconds and the time it takes to scroll -->
	<Carousel {images} onchange={(detail) => (image = detail)} duration={4000}>
		<Controls />
		<CarouselIndicators />
	</Carousel>

	<div class="my-2 h-10 rounded-sm bg-gray-300 p-2 text-center dark:bg-gray-700 dark:text-white">
		{image?.alt}
	</div>
</div>
