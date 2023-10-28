<script>
	import DetailedInfomation from "../../components/DetailedInfomation.svelte";
	const title = "Außenbereich";
	const infoText =
		"Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet. Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua. At vero eos et accusam et justo duo dolores et ea rebum. Stet clita kasd gubergren, no sea takimata sanctus est Lorem ipsum dolor sit amet.";
	const imageInfos = [
		{
			path: "/placeholder.jpg",
			alt: "Bild aus der Schreinerei"
		},
		{
			path: "/placeholder.jpg",
			alt: "Bild aus der Schreinerei"
		},
		{
			path: "/placeholder.jpg",
			alt: "Bild aus der Schreinerei"
		}
	];
</script>

<DetailedInfomation {title} {infoText} {imageInfos} />
