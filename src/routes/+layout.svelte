<script>
	import { page } from "$app/stores";
	import "../app.css";
	import Abschlusstext from "../components/Abschlusstext.svelte";
	import Address from "../components/Address.svelte";
	import Footer from "../components/Footer.svelte";
	import Header from "../components/Header.svelte";
	import Navigation from "../components/Navigation.svelte";
	const routes = [
		{ name: "Über Uns", path: "/" },
		{ name: "Projekte", path: "/projects" }
	];
</script>

<div
	class="flex flex-row justify-center items-start text-dark-gray dark:bg-dark-gray dark:text-white">
	<div class="w-full xl:w-3/4 dark:bg-dark-gray">
		<Navigation />
		<Header />
		<slot />
		<Abschlusstext />
		<Address />
		<Footer />
	</div>
</div>
