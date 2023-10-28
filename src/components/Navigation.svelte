<script>
	import { page } from "$app/stores";
	import "../app.css";
	import Burger from "./Icons/Burger.svelte";
	import X from "./Icons/X.svelte";
	const routes = [
		{ name: "Über Uns", path: "/" },
		{ name: "Projekte", path: "/projects" }
	];

	let showNavigation = false;

	function toggleShowNavigation() {
		showNavigation = !showNavigation;
	}
</script>

<div class="flex flex-col bg-mendel-blue text-white sticky top-0 md:hidden">
	<div class="w-full h-12 sticky top-0 flex flex-row justify-between items-center px-4">
		<img src="/icon-white.png" alt="Logo der Schreinerei Mendel" class="w-8 h-8 object-contain" />
		<button on:click={toggleShowNavigation}>
			{#if showNavigation}
				<X />
			{:else}
				<Burger />
			{/if}
		</button>
	</div>
	{#if showNavigation}
		<nav class="bg-mendel-blue flex flex-col m-8 animate">
			{#each routes as route}
				<a
					class="py-2 text-xl font-bold transition-all rounded"
					href={route.path}
					class:active={$page.url.pathname === route.path}>{route.name}</a>
			{/each}
		</nav>
	{/if}
</div>

<div class="flex-col bg-mendel-blue text-white sticky top-0 hidden md:flex">
	<div class="flex flex-row justify-between items-center px-4">
		<div class="w-1/4">
			<img src="/icon-white.png" alt="Logo der Schreinerei Mendel" class="w-8 h-8 object-contain" />
		</div>
		<nav class="bg-mendel-blue flex flex-row justify-center items-center m-2 gap-2 w-2/4">
			{#each routes as route}
				<a
					class="py-1 px-4 transition-all rounded"
					href={route.path}
					class:default-active={$page.url.pathname === route.path}>{route.name}</a>
			{/each}
		</nav>
		<div class="w-1/4" />
	</div>
</div>

<style>
	a.active {
		padding-left: 20px;
		transition: 1s ease;
		background-color: rgb(0, 0, 0, 0.25);
	}
	a.default-active {
		transition: 1s ease;
		background-color: rgb(0, 0, 0, 0.25);
	}
	/* Define the animation */
	@keyframes slidein {
		0% {
			transform: translateY(-100%);
			opacity: 0;
		}
		100% {
			transform: translateY(0%);
			opacity: 1;
		}
	}

	/* Apply the animation to the image when a certain class is added */
	.animate {
		animation: slidein 1s cubic-bezier(0.075, 0.82, 0.165, 1);
	}
</style>
