<script>
	export let title = "";
	export let optionText = "";
	export let icon = "";
	//export let iconWhite = "";
</script>

<div class="flex flex-row justify-start items-start p-4 lg:p-8 lg:w-[50%]">
	<img src={icon} alt="icon" class="w-8 h-8 mr-4" />
	<div class="flex flex-col justify-start items-start">
		<p class="pb-2 font-bold leading-none text-mendel-blue text-2xl">{title}</p>
		<p class="text-sm">{optionText}</p>
	</div>
</div>
