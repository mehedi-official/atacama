<script lang="ts">
	import Navbar from '@components/Navbar.svelte';
	import avatar_01 from '$lib/assets/avatar_01.png';
	import avatar_02 from '$lib/assets/avatar_02.png';
	import avatar_03 from '$lib/assets/avatar_03.png';
	import volunteer from '$lib/assets/volunteer.png';
	import { refresh, refresh_temp } from '$lib/Icons.svelte';
	import Project from '@components/Project.svelte';
	import Initiative from '@components/Initiative.svelte';
	import Problem from '@components/Problem.svelte';
	import Footer from '@components/Footer.svelte';
</script>

<header class="p-6">
	<Navbar />
	<section class="mt-5 grid grid-cols-2 gap-5">
		<section class="bg-primary text-black-800 rounded-2xl px-12 py-36 text-center">
			<div>
				<p>Atacama Group</p>
				<h1 class="text-6xl">Saving Nature & Fighting Climate Change Together.</h1>
			</div>
			<div class="mt-8">
				<div class="flex justify-center gap-3">
					<input
						class=" block rounded-full bg-white/40 px-5 py-4"
						type="email"
						placeholder="Enter your email"
					/>
					<button class="rounded-full bg-white px-5 py-4">Subscribe</button>
				</div>
				<div class="mt-5 flex items-center justify-center gap-3">
					<div class="flex items-center select-none">
						<span class="h-8 w-8 overflow-hidden rounded-full border-2 border-white bg-gray-500"
							><img src={avatar_01} alt="Avatar 01" /></span
						>
						<span
							class="-ml-2 h-8 w-8 overflow-hidden rounded-full border-2 border-white bg-gray-500"
							><img src={avatar_02} alt="Avatar 01" /></span
						>
						<span
							class="-ml-2 h-8 w-8 overflow-hidden rounded-full border-2 border-white bg-gray-500"
							><img src={avatar_03} alt="Avatar 01" /></span
						>
					</div>
					<p class="max-w-48 text-left">1.7M+ members of our charity organization</p>
				</div>
			</div>
		</section>
		<section class="bg relative rounded-2xl p-8">
			<section class="flex items-start justify-between">
				<div class="grid max-w-56 grid-cols-2 items-end gap-3 rounded-xl bg-white p-3">
					<div class="h-28.5 w-22.5 overflow-hidden rounded-xl">
						<img src={volunteer} alt="volunteer" class="h-full w-full object-cover" />
					</div>
					<div>
						<span class="border-primary inline-flex rounded-full border p-0.5">
							<span class="bg-primary inline-block h-2 w-2 rounded-full"></span>
						</span>
						<p>We & Our Volunteers</p>
					</div>
				</div>

				<div class="inline-flex rounded-full border border-white/60 bg-white/30 p-2">
					{@render refresh()}
				</div>
			</section>

			<div class="absolute top-2/6 right-1/6 flex items-center gap-2">
				<span class="border-primary inline-flex rounded-full border p-1">
					<span class="bg-primary inline-block h-2 w-2 rounded-full"></span>
				</span>
				<span
					class="border-primary text-primary inline-flex items-center rounded-full border px-2.5 py-2"
					>GHG Emissions</span
				>
			</div>

			<div class="absolute top-2/5 left-1/6 flex items-center gap-2">
				<span class="border-primary inline-flex rounded-full border p-1">
					<span class="bg-primary inline-block h-2 w-2 rounded-full"></span>
				</span>
				<span
					class="border-primary text-primary inline-flex items-center rounded-full border px-2.5 py-2"
					>Ocean Polution</span
				>
			</div>

			<div class="absolute top-3/5 left-1/2 flex items-center gap-2">
				<span class="border-primary inline-flex rounded-full border p-1">
					<span class="bg-primary inline-block h-2 w-2 rounded-full"></span>
				</span>
				<span
					class="border-primary text-primary inline-flex items-center rounded-full border px-2.5 py-2"
					>Deforestation</span
				>
			</div>

			<div class="absolute bottom-4 left-8 w-fit rounded-xl bg-white">
				<div class="relative px-4 py-3">
					<p class="max-w-44 text-center">Join us in fighting environmental problems</p>
					<span class="bg-primary absolute top-2 left-2 flex h-2.5 w-2.5 rounded-full"></span>
					<span class="bg-primary absolute top-2 right-2 flex h-2.5 w-2.5 rounded-full"></span>
				</div>
			</div>

			<div class="flex items-center gap-3">
				<div class="flex gap-0.5">
					<div class="border-primary flex h-9 w-9 items-center justify-center rounded-full border">
						{@render refresh_temp()}
					</div>
					<div class="border-primary flex h-9 w-9 items-center justify-center rounded-full border">
						{@render refresh_temp()}
					</div>
				</div>
				<p class="text-primary">Find us on social networks</p>
			</div>
		</section>
	</section>
</header>
<Project />
<Initiative />
<Problem />
<Footer />

<style>
	.bg {
		background: url('$lib/assets/header_bg.avif');
		background-size: cover;
	}
</style>
