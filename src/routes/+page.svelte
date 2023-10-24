<script>
	import Address from "../components/Address.svelte";
	import Introduction from "../components/Introduction.svelte";
	import Option from "../components/Option.svelte";
	import { texts } from "../info/options";
</script>

<div>
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
</div>
