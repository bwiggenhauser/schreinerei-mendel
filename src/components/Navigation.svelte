<script>
	import { page } from "$app/stores";
	const routes = [
		{ name: "Über Uns", path: "/" },
		{ name: "Projekte", path: "/projects" }
	];

	let showNavigation = false;

	function toggleShowNavigation() {
		showNavigation = !showNavigation;
	}
</script>

<div class="bg-gray h-12 w-full flex flex-row justify-end items-center pr-4">
	<button on:click={toggleShowNavigation}>
		<p>Toggle</p>
	</button>
</div>
