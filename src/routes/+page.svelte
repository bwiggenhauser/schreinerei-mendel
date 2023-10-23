<script>
	import "../app.css";
	import Address from "../components/Address.svelte";
	import Header from "../components/Header.svelte";
	import Introduction from "../components/Introduction.svelte";
	import Option from "../components/Option.svelte";
	import { texts } from "../info/options";
</script>

<div class="dark:bg-black dark:text-white">
	<Header />
	<Introduction />
	{#each texts as option}
		<Option title={option.title} optionText={option.text} icon={option.icon} />
	{/each}
	<Address />
</div>

<style>
</style>
