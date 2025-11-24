<script lang="ts">
	import { Carousel, Controls, CarouselIndicators } from 'flowbite-svelte';
	import type { HTMLImgAttributes } from 'svelte/elements';

	const { images } = $props();

	let index = $state(0);
	// start with the first image if available
	let image: HTMLImgAttributes | undefined = $state(images?.[0]);
</script>

<div class="mx-auto max-w-6xl p-4">
	<!-- glass card so gradient shows through -->
	<div class="relative overflow-hidden rounded-2xl bg-white/10 shadow-2xl ring-1 ring-white/10 backdrop-blur-sm dark:bg-black/20">
		<!-- size the carousel; adjust h-64 / sm:h-96 to taste -->
		<Carousel class="h-64 w-full sm:h-96" {images} onchange={(detail) => (image = detail)} duration={4000}>
			<Controls />
			<!-- floating caption centered above the indicators -->
			<div class="absolute bottom-12 left-1/2 z-20 -translate-x-1/2">
				<div class="rounded-full border border-white/20 bg-white/30 px-4 py-2 text-sm text-white shadow-md backdrop-blur-md dark:bg-black/40">
					{image?.alt}
				</div>
			</div>
			<CarouselIndicators />
		</Carousel>
	</div>
</div>
