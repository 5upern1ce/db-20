<script lang="ts">
	import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte';
</script>

<div class="bg-yellow-100">
	<Navbar>
		<NavBrand href="/">
			<img src="/DB20_logo.jpg" class="me-3 h-10 align-middle sm:h-15" alt="DB2.0" />
			<!-- <span class="self-center text-3xl font-extrabold whitespace-nowrap text-green-600 dark:text-green-900">DB</span>
		<span class="inline-block self-center bg-gradient-to-t from-orange-800 via-orange-700 to-orange-300 bg-clip-text text-3xl font-extrabold whitespace-nowrap text-transparent">2.0</span> -->
		</NavBrand>
		<NavHamburger />
		<NavUl class="">
			<NavLi href="/">Home</NavLi>
			<NavLi href="/about">About</NavLi>
			<NavLi href="/docs/components/navbar">Navbar</NavLi>
			<NavLi href="/pricing">Pricing</NavLi>
			<NavLi href="/contact">Contact</NavLi>
		</NavUl>
	</Navbar>
</div>
