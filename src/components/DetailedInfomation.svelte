<script>
	export let title = "";
	export let infoText = "";
	export let imageInfos = [];
</script>

<div class="">
	<div class="p-4">
		<h1 class="text-5xl font-bold text-center mb-2">{title}</h1>
		<p class="text-center">{infoText}</p>
	</div>
	<div class="flex flex-col md:flex-row flex-wrap justify-center gap-4 p-4">
		{#each imageInfos as image}
			<img
				src={image.path}
				alt={image.alt}
				class="w-full md:w-2/5 h-auto object-contain shadow-lg rounded-xl" />
		{/each}
	</div>
</div>
