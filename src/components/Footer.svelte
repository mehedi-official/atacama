<script>
	import { arrow_right } from "$lib/Icons.svelte";

</script>
<footer class="mt-9 bg-neutral-50 px-12">
	<section class="grid grid-cols-[1fr_3fr] items-start gap-48 py-16">
		<h5
			class="text-black-700 text-lg/none font-medium flex w-fit items-center justify-center rounded-full border border-gray-100 px-3.5 py-2"
		>
			Newsletter
		</h5>

		<section class="justify-self-end">
			<h6 class="text-black-800 text-[2.125rem]/[1.2]">
				Subscribe to our newsletter to get the latest updates on mission projects & initiatives.
			</h6>
			<div class="mt-6 flex items-center gap-4">
				<input
					class="text-black-800 font-medium flex h-12 w-full items-center rounded-full bg-white px-4 py-2 placeholder:text-gray-200"
					type="email"
					placeholder="Email Address"
				/>
				<button
					class="bg-primary hover:underline underline-offset-2 font-medium text-black-800 flex gap-2 h-12 cursor-pointer items-center rounded-full pl-4 pr-2.5 py-2"
					>Subscribe <span class="w-5 h-5">{@render arrow_right()}</span></button
				>
			</div>
		</section>
	</section>

	<section
		class="flex items-center justify-between border-t border-gray-100 pt-9 pb-6 text-base/none text-gray-200"
	>
		<p>© {new Date().getFullYear()}. All rights Reserved.</p>

		<div>Atacama</div>

		<div class="flex items-center">
			<button
				class="flex w-fit items-center justify-center rounded-full border cursor-pointer hover:bg-gray-100/20 border-gray-100 px-3.5 py-2"
				>Facebook</button
			>
			<button
				class="flex w-fit items-center justify-center rounded-full cursor-pointer hover:bg-gray-100/20 border border-gray-100 px-3.5 py-2"
				>Twitter</button
			>
			<button
				class="flex w-fit items-center justify-center rounded-full cursor-pointer hover:bg-gray-100/20 border border-gray-100 px-3.5 py-2"
				>Instagram</button
			>
		</div>
	</section>
</footer>
