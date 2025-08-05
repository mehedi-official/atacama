<script lang="ts">
	import ProblemCard from './ProblemCard.svelte';
	import forest from "$lib/assets/japan.avif";
	import ocean from "$lib/assets/atacama_desert.avif";
	import emission from "$lib/assets/laguna verde.jpg";
	import mountain from "$lib/assets/mountain.avif";
	let activeCardIdx = $state.raw(0);

	let data = [
		{ title: 'Ocean Pollution', description: 'Millions of tons of plastic threaten the lives of aquatic animals and ecosystem.', img: ocean},
		{ title: 'Glacier Melting', description: 'Due to melting glaciers and warming, the habitat of animals and insects are changing.', img: mountain},
		{ title: 'Forest Clearance', description: 'Forests are disappearing, and with them unique species of plants and animals.', img: forest},
		{ title: 'GHG Emissions', description: "Excessive greenhouse gas emissions lead to climate disasters. Greenhouse gas emissions trap the sun's heat", img: emission}
	]

	function renderColumn(activeIndex: number): string {
		switch (activeIndex) {
			case 0:
				return 'grid-cols-[1.65fr_1fr_1fr_1fr]';
			case 1:
				return 'grid-cols-[1fr_1.65fr_1fr_1fr]';
			case 2:
				return 'grid-cols-[1fr_1fr_1.65fr_1fr]';
			case 3:
				return 'grid-cols-[1fr_1fr_1fr_1.65fr]';
			default:
				return 'grid-cols-[1.65fr_1fr_1fr_1fr]';
		}
	}
</script>

<section class={[renderColumn(activeCardIdx), "grid min-h-150 gap-4 px-6 pt-14 pb-9"]}>
	{#each data as { title, description, img }, idx }
		<ProblemCard --bg-img={`url(${img})`} isActive={idx === activeCardIdx} {title} {description}/>
	{/each}
</section>
