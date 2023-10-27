<div class="flex flex-col justify-start items-center font-bold mb-6">
	<div class="image-container animate mt-8">
		<img src="/icon_new.png" alt="Schreinerei Icon" />
	</div>
	<h1 class="text-4xl lg:text-6xl animate mt-6 leading-none text-center mb-2">
		Schreinerei Mendel
	</h1>
	<div class="flex flex-row w-full justify-evenly animate">
		<p class="text-gray-600 dark:text-gray-300">Meister- und Ausbildungsbetrieb</p>
	</div>
</div>

<style>
	.image-container {
		width: 200px; /* Adjust the width and height as per your requirements */
		height: auto;
		overflow: hidden; /* Ensures the image doesn't overflow the container */
	}

	/* Define the animation */
	@keyframes slidein {
		0% {
			transform: translateY(-100%);
			opacity: 0;
		}
		100% {
			transform: translateY(0%);
			opacity: 1;
		}
	}

	/* Apply the animation to the image when a certain class is added */
	.animate {
		animation: slidein 1s cubic-bezier(0.075, 0.82, 0.165, 1);
	}
</style>
