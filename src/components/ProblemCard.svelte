<script>
	import { arrow_right } from '$lib/Icons.svelte';
	let { isActive = false } = $props();
</script>

<section class="flex h-full flex-col justify-between gap-6 overflow-hidden rounded-2xl p-3.5">
	<div class={[isActive || 'justify-end', 'flex items-start justify-between gap-2']}>
		{#if isActive}
			<div>
				<div class="flex items-center">
					<span class="border-primary inline-flex rounded-full border p-1.5">
						<span class="bg-primary inline-block h-3.5 w-3.5 rounded-full"></span>
					</span>
					<span
						class="border-primary text-primary inline-flex items-center rounded-full border px-2.5 py-2"
						>Ecological Catastrophy</span
					>
				</div>

				<div class="flex items-center">
					<span
						class="border-primary text-primary inline-flex items-center rounded-full border px-2.5 py-2"
						>Pollution Issues</span
					>
					<span class="border-primary inline-flex rounded-full border p-1.5">
						<span class="bg-primary inline-block h-3.5 w-3.5 rounded-full"></span>
					</span>
				</div>
			</div>
		{/if}
		<button
			class={[
				isActive ? 'bg-primary' : '-rotate-45 bg-white',
				'flex aspect-square w-14 rounded-full p-3'
			]}>{@render arrow_right()}</button
		>
		<!-- class="w-full flex " -->
	</div>
	<div>
		<div class="flex flex-col gap-3 px-2.5 text-white">
			<h3>Forest Clearance</h3>
			<p>Forests are disappearing, and with them unique species of plants and animals.</p>
		</div>
		<button class="mt-5 flex w-full rounded-full bg-white px-6 py-4.5">EXPLORE PROBLEM</button>
	</div>
</section>

<style>
	section {
		background: url('$lib/assets/ice_mountain.avif');
		background-size: cover;
	}
</style>
