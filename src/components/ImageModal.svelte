<!-- ImageModal.svelte -->
<script lang="ts">
	export let imageUrl: string;
	export let closeModal: () => void;
</script>

<div class="modal" on:click={closeModal} on:keydown={closeModal} role="button" tabindex="0">
	<!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
	<div
		class="modal-content rounded-lg p-1 md:p-4 shadow-xl bg-white w-4/5 md:h-4/5 md:w-fit"
		on:click|stopPropagation
		on:keydown|stopPropagation
		role="dialog">
		<!-- svelte-ignore a11y-missing-attribute -->
		<img src={imageUrl} class="object-cover md:h-full rounded-lg" />
	</div>
</div>

<style>
	.modal {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		background-color: rgba(0, 0, 0, 0.5);
		display: flex;
		justify-content: center;
		align-items: center;
	}
</style>
