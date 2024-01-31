<script>
	import DetailedInfomation from "../../components/DetailedInfomation.svelte";

	const data = [
		{
			title: "Möbelbau",
			path: "/gallery/moebel",
			index: ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"]
		},
		{
			title: "Innenausbau",
			path: "/gallery/innenausbau",
			index: ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"]
		},
		{
			title: "Bodenbeläge",
			path: "/gallery/boden",
			index: ["1", "2", "3", "4", "5", "6"]
		},
		{
			title: "Außenbereich",
			path: "/gallery/aussenbereich",
			index: ["1", "2", "3", "4", "5", "6", "7", "8", "9", "10", "11"]
		},
		{
			title: "Renovierungsarbeiten",
			path: "/gallery/renovierung",
			index: ["1", "2", "3", "4", "5", "6"]
		}
	];
</script>

<div class="flex flex-col gap-4 px-4 text-sm text-center items-center">
	{#each data as item}
		<DetailedInfomation path={item.path} indices={item.index} title={item.title} />
	{/each}
</div>
