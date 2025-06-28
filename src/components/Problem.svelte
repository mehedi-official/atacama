<script>
	import ProblemCard from './ProblemCard.svelte';
</script>

<section class="grid min-h-150 grid-cols-[1.65fr_1fr_1fr_1fr] gap-4 px-6 pt-14 pb-9">
	<ProblemCard isActive={true} />
	<ProblemCard />
	<ProblemCard />
	<ProblemCard />
</section>
