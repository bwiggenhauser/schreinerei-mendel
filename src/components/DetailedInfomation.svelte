<script>
	export let title = "";
	export let path = "";
	export let indices = [];
	const x = "max-w-1/5 md:w-2/5 object-cover shadow-lg rounded-xl hover:scale-125 transition-all";
</script>

<div class="">
	<div class="p-4">
		<h1 class="text-3xl font-bold text-center">{title}</h1>
	</div>
	<div class="flex flex-row flex-wrap gap-4 justify-center">
		{#each indices as index}
			<img
				src={path + "/" + index + ".jpg"}
				alt="empty"
				class="md:w-64 md:h-64 h-auto w-full object-cover rounded-lg md:hover:scale-150 md:transition-all" />
		{/each}
	</div>
</div>
