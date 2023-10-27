<script>
	import Address from "../components/Address.svelte";
	import Introduction from "../components/Introduction.svelte";
	import NewIntroduction from "../components/NewIntroduction.svelte";
	import Option from "../components/Option.svelte";
	import { texts } from "../info/options";
</script>

<div>
	<Introduction />
	<h1 class="text-center text-3xl font-bold mt-8 mb-4">Unsere Leistungen</h1>
	<div class="flex flex-col lg:flex-row flex-wrap lg:justify-center">
		{#each texts as option}
			<Option title={option.title} optionText={option.text} icon={option.icon} />
		{/each}
	</div>
</div>
