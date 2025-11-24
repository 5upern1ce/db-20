<script lang="ts">
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
	import Facebook from './assets/Facebook.svelte';
</script>

<div class="bg-gradient-to-r from-orange-400 via-orange-300 to-green-200 shadow-md">
	<Navbar class="mx-auto max-w-7xl px-4 py-3 sm:px-6 lg:px-8">
		<!-- Brand -->
		<NavBrand href="/" class="flex items-center gap-3">
			<img src="/DB20_logo.jpg" class="h-12 rounded-md object-cover ring-2 ring-green-700/40" alt="DB2.0" />
			<div class="leading-tight">
				<span class="self-center text-3xl font-extrabold whitespace-nowrap text-green-600 dark:text-green-900">DB</span>
				<span class="inline-block self-center bg-gradient-to-t from-orange-800 via-orange-700 to-orange-300 bg-clip-text text-3xl font-extrabold whitespace-nowrap text-transparent">2.0</span>
				<span class="block text-sm font-bold tracking-wide text-orange-800">Independant Skate Shop</span>
			</div>
		</NavBrand>

		<NavHamburger />
		<NavUl class="font-bold">
			<!-- Each href is the pages on the navbar, just add another -->
			<NavLi href="/">Home</NavLi>
			<NavLi href="/about">About</NavLi>
			<NavLi href="/contact">Contact</NavLi>
		</NavUl>
	</Navbar>
</div>
