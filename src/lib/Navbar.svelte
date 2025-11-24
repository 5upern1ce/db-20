<script lang="ts">
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
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

		<!-- Mobile hamburger -->
		<NavHamburger class="text-green-900 hover:text-orange-800" />

		<!-- Nav items (pushed right with ml-auto) -->
		<NavUl class="ml-auto flex items-center space-x-2">
			<NavLi href="/" class="rounded px-3 py-2 font-semibold text-green-900 transition hover:bg-green-900/10 hover:text-green-800">Home</NavLi>
			<NavLi href="/about" class="rounded px-3 py-2 font-semibold text-green-900 transition hover:bg-green-900/10 hover:text-green-800">About</NavLi>
		</NavUl>
	</Navbar>
</div>
