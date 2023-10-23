<script>
	import "../app.css";
	import Address from "../components/Address.svelte";
	import Header from "../components/Header.svelte";
	import Introduction from "../components/Introduction.svelte";
	import Option from "../components/Option.svelte";
	import { texts } from "../info/options";
</script>

<div class="flex flex-row justify-center items-start dark:bg-black dark:text-white scroll-smooth">
	<div class="w-full lg:w-2/3 dark:bg-neutral-800">
		<Header />
		<Introduction />
		<div class="flex flex-col lg:flex-row flex-wrap">
			{#each texts as option}
				<Option
					title={option.title}
					optionText={option.text}
					icon={option.icon}
					iconWhite={option.iconWhite} />
			{/each}
		</div>
		<Address />
	</div>
</div>

<style>
</style>
