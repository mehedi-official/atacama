<script>
	import { arrow_right } from '$lib/Icons.svelte';
</script>

<section class="px-6 pt-13 pb-14">
	<div class="flex items-center justify-between">
		<h2>Our initiatives for {new Date().getFullYear()}</h2>
		<p class="max-w-68">Find out what projects we are implementing to protect nature</p>
	</div>

	<section class="mt-12">
		<div class="grid grid-cols-[1.75fr_1.5fr_1.5fr_1fr] gap-1.5 pb-6 text-gray-200">
			<h4>Title</h4>
			<h4>Tags</h4>
			<h4>Date</h4>
			<div></div>
		</div>

		<div
			class="grid grid-cols-[1.75fr_1.5fr_1.5fr_1fr] items-center gap-1.5 border-t border-gray-200 py-8"
		>
			<h4>Tree Planting</h4>
			<span class="inline-flex w-fit rounded-full border border-gray-100 px-4 py-2"
				>green & cleaner</span
			>
			<p>
				{new Date().toLocaleDateString('en-GB', {
					day: '2-digit',
					month: '2-digit',
					year: '2-digit'
				})}
			</p>
			<button
				class="flex aspect-square w-14 items-center justify-center justify-self-end rounded-full bg-neutral-50 p-3.5"
				>{@render arrow_right()}</button
			>
		</div>

		<div
			class="grid grid-cols-[1.75fr_1.5fr_1.5fr_1fr] items-center gap-1.5 border-t border-gray-200 py-8"
		>
			<h4>Beach Cleanup</h4>
			<span class="inline-flex w-fit rounded-full border border-gray-100 px-4 py-2"
				>future generations</span
			>
			<p>
				{new Date().toLocaleDateString('en-GB', {
					day: '2-digit',
					month: '2-digit',
					year: '2-digit'
				})}
			</p>
			<button
				class="flex aspect-square w-14 items-center justify-center justify-self-end rounded-full bg-neutral-50 p-3.5"
				>{@render arrow_right()}</button
			>
		</div>

		<div
			class="grid grid-cols-[1.75fr_1.5fr_1.5fr_1fr] items-center gap-1.5 border-t border-gray-200 py-8"
		>
			<h4>Educational Events</h4>
			<span class="inline-flex w-fit rounded-full border border-gray-100 px-4 py-2">courses</span>
			<p>
				{new Date().toLocaleDateString('en-GB', {
					day: '2-digit',
					month: '2-digit',
					year: '2-digit'
				})}
			</p>
			<button
				class="flex aspect-square w-14 items-center justify-center justify-self-end rounded-full bg-neutral-50 p-3.5"
				>{@render arrow_right()}</button
			>
		</div>

		<div
			class="grid grid-cols-[1.75fr_1.5fr_1.5fr_1fr] items-center gap-1.5 border-t border-gray-200 py-8"
		>
			<h4>Park Cleaning</h4>
			<span class="inline-flex w-fit rounded-full border border-gray-100 px-4 py-2"
				>day off cleaning</span
			>
			<p>
				{new Date().toLocaleDateString('en-GB', {
					day: '2-digit',
					month: '2-digit',
					year: '2-digit'
				})}
			</p>
			<button
				class="flex aspect-square w-14 items-center justify-center justify-self-end rounded-full bg-neutral-50 p-3.5"
				>{@render arrow_right()}</button
			>
		</div>
	</section>
</section>
