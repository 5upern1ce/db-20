<script lang="ts">
	import { page } from '$app/state';
</script>

<div class="grid w-full justify-items-center">
	<h1 class="col-span-3 flex justify-center pt-6 text-5xl font-bold">{page.status}</h1>
	<h2 class=" col-span-3 flex justify-center pb-4 text-2xl font-bold">{page.error.message}</h2>
	<a class=" col-span-3 flex h-full w-1/2 max-w-[400px] justify-center rounded-md bg-blue-500 bg-gradient-to-t from-orange-800 via-orange-700 to-orange-300 object-cover px-4 py-2 pt-3 text-center font-bold text-wrap text-white ring-2 ring-gray-300/40 hover:bg-blue-700" href="/"> Return to the home page </a>
</div>
