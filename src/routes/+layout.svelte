<script>
	import "../app.css";
	import Navigation from "../components/Navigation.svelte";
</script>

<div class="flex flex-row justify-center items-start scroll-smooth">
	<slot />
</div>

<style>
	a.active {
		background-color: rgba(0, 0, 0, 0.24);
		transition: 0.5s all;
	}
</style>
