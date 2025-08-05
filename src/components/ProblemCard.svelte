<script lang="ts">
	import { arrow_right } from '$lib/Icons.svelte';
	import {  } from "$lib/assets/japan.avif";
	let { isActive = false, title, description }: { isActive: boolean, title: string, description: string } = $props();
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
						class="border-primary text-base/none text-primary inline-flex items-center rounded-full border px-2.5 py-1.5"
						>Ecological Catastrophy</span
					>
				</div>

				<div class="flex items-center">
					<span
						class="border-primary text-base/none text-primary inline-flex items-center rounded-full border px-2.5 py-1.5"
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
				isActive ? 'bg-primary' : '-rotate-45 bg-white hover:bg-primary hover:rotate-0',
				'flex transition-all duration-200 cursor-pointer aspect-square w-14 rounded-full p-3'
			]}>{@render arrow_right()}</button
		>
	</div>
	<div>
		<div class="flex flex-col gap-2 px-2.5 text-white">
			<h3 class="text-4xl font-medium">{title}</h3>
			<p class="text-sm/tight">{description}</p>
		</div>
		<button class="mt-5 cursor-pointer transition-all duration-300 hover:bg-primary font-medium flex items-center gap-3 justify-between w-full rounded-full bg-white px-6 py-4.5">EXPLORE PROBLEM <span class="w-4.5 aspect-square">{@render arrow_right()}</span></button>
	</div>
</section>

<style>
	section {
		background-image: var(--bg-img);
		background-size: cover;
	}
</style>
