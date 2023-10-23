<script>
	export let title = "";
	export let optionText = "";
	export let icon = "";
	export let iconWhite = "";
</script>

<div class="flex flex-row justify-start items-start p-4 lg:p-8 lg:w-[50%]">
	<img src={icon} alt="icon" class="w-8 h-8 mr-4 dark:hidden" />
	<img src={iconWhite} alt="icon" class="w-8 h-8 mr-4 hidden dark:block" />
	<div class="flex flex-col justify-start items-start">
		<p class="pb-1 font-bold leading-none">{title}</p>
		<p class="text-sm">{optionText}</p>
	</div>
</div>
