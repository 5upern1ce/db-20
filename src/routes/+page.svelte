<script>
	import Navbar from '$lib/Navbar.svelte';
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
			alt: 'New wheels from Sushi, Slimeballs, Santa Cruz and More',
			src: '/home-carousel-images/new-wheels-oct-17.jpg',
			title: 'New wheels just in!'
		}
	];
</script>

<Navbar />

<!-- full width row, center the inner fixed-width box -->
<div class="flex w-full justify-center pt-3">
	<div class="w-[800px] max-w-full">
		<Carousel {images} />
	</div>
</div>
