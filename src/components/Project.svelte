<script lang="ts">
	import ice_mountain from '$lib/assets/ice_mountain.avif';
	import desert_mountain from '$lib/assets/ice_mountain.avif';
</script>

<section class="px-6 pt-21 pb-13">
	<article class="relative">
		<div class="mx-auto max-w-140">
			<div class="mb-5 grid gap-6 text-center">
				<h2 class="text-5xl">Let's Make Our World Cleaner & Greener!</h2>
				<p class="px-24">
					We work with partners & communities to ensure nature thrives and climate change is
					reversed
				</p>
			</div>
			<div class="flex items-center justify-center gap-8">
				<a
					href="/"
					class="inline-flex rounded-full border border-gray-100 px-5 py-4 leading-none text-black"
					>View Projects</a
				>
				<a href="/" class="inline-flex items-center gap-2.5 text-black hover:underline"
					><span class="bg-primary inline-flex h-2 w-2 rounded-full"></span>Learn More</a
				>
			</div>
		</div>

		<div class="absolute top-12 left-1/8 inline-grid gap-2">
			<img
				src={ice_mountain}
				alt="1"
				class="border-primary aspect-square w-16 rounded-full border-2 object-cover"
			/>
			<img
				src={ice_mountain}
				alt="1"
				class=" border-primary ml-20 aspect-square w-16 rounded-full border-2 object-cover"
			/>
		</div>

		<div class="absolute top-12 right-1/8 inline-grid justify-items-end gap-2">
			<img
				src={ice_mountain}
				alt="1"
				class="border-primary aspect-square w-16 rounded-full border-2 object-cover"
			/>
			<img
				src={ice_mountain}
				alt="1"
				class="border-primary mr-20 aspect-square w-16 rounded-full border-2 object-cover"
			/>
		</div>
	</article>

	<section class="mt-28 grid grid-cols-4">
		<div class="relative aspect-3/2 overflow-hidden rounded-full">
			<div class="h-full bg-neutral-50"></div>
			<p class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">We</p>
		</div>
		<div class="relative overflow-hidden rounded-full">
			<img src={ice_mountain} alt="Ice mountain" class="block h-full" />
			<p class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 text-white">Protect</p>
		</div>
		<div class="relative overflow-hidden rounded-full">
			<div class="bg-primary h-full"></div>
			<p class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
				<svg
					width="184"
					height="184"
					viewBox="0 0 184 184"
					fill="none"
					xmlns="http://www.w3.org/2000/svg"
				>
					<path
						d="M38.332 92H145.665"
						stroke="black"
						stroke-width="10"
						stroke-linecap="round"
						stroke-linejoin="round"
					/>
					<path
						d="M92 38.333L145.667 91.9997L92 145.666"
						stroke="black"
						stroke-width="10"
						stroke-linecap="round"
						stroke-linejoin="round"
					/>
				</svg>
			</p>
		</div>
		<div class="relative overflow-hidden rounded-full">
			<img src={desert_mountain} alt="Desert mountain" class="block h-full" />
			<p class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 text-white">Nature</p>
		</div>
	</section>
</section>
