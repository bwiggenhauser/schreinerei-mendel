<script>
	import { page } from "$app/stores";
	import "../app.css";
	import Abschlusstext from "../components/Abschlusstext.svelte";
	import Address from "../components/Address.svelte";
	import Footer from "../components/Footer.svelte";
	import Header from "../components/Header.svelte";
	const routes = [
		{ name: "Über Uns", path: "/" },
		{ name: "Projekte", path: "/projects" }
	];
</script>

<div
	class="flex flex-row justify-center items-start dark:bg-dark-gray dark:text-white scroll-smooth">
	<div class="w-full md:w-3/4 lg:w-2/3 xl:w-1/2 dark:bg-dark-gray">
		<nav
			class="bg-mendel-blue flex flex-col items-center gap-x-16 md:py-2 md:flex-row md:justify-center sticky top-0">
			{#each routes as route}
				<a
					class="py-1 px-4 text-white w-full text-center md:w-fit md:rounded-xl"
					href={route.path}
					class:active={$page.url.pathname === route.path}>{route.name}</a>
			{/each}
		</nav>
		<Header />
		<slot />
		<Abschlusstext />
		<Address />
		<Footer />
	</div>
</div>

<style>
	a.active {
		background-color: rgba(0, 0, 0, 0.24);
		transition: 0.5s all;
	}
</style>
