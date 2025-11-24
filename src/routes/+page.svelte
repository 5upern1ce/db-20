<script>
	import Carousel from '$lib/Carousel.svelte';

	const images = [
		// 'alt' is the text displayed below the image
		// 'src' is the image itself
		// 'title' is the actual alt texts
		{
			alt: 'Heathen, Krooked, Anti-Hero and Bird House',
			src: '/home-carousel-images/skateboards-june-25.jpg',
			title: 'Skateboards in the shop'
		},
		{
			alt: 'New wheels from Sushi, Slimeballs, Santa Cruz and More ',
			src: '/home-carousel-images/new-wheels-oct-17.jpg',
			title: 'New wheels just in!'
		}
	];
</script>

<!-- full width row, center the inner fixed-width box -->
<h1 class="m-2 flex w-full justify-center pt-3 text-5xl">
	Welcome to <span class=" self-center pl-1 text-6xl font-extrabold whitespace-nowrap text-green-600 dark:text-green-900">DB</span>
	<span class="inline-block self-center bg-gradient-to-t from-orange-800 via-orange-700 to-orange-300 bg-clip-text text-6xl font-extrabold whitespace-nowrap text-transparent">2.0</span>
</h1>
<div class="flex w-full justify-center pt-3">
	<div class="w-[800px] max-w-full">
		<Carousel {images} />
	</div>
</div>
