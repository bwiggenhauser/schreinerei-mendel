<script>
	export let title = "";
	export let optionText = "";
	export let icon = "";
</script>

<div class="flex flex-row justify-start items-start m-4">
	<img src={icon} alt="icon" class="w-6 h-6 mr-4 dark:fill-white" />
	<div class="flex flex-col justify-start items-start">
		<p class="pb-1 font-bold">{title}</p>
		<p class="text-sm">{optionText}</p>
	</div>
</div>
