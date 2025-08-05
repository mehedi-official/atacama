<nav class="flex justify-between gap-4">
	<ul class="flex items-center gap-2">
		<li class="btn flex items-center gap-2"><span class="flex w-2 h-2 rounded-full bg-black-800"></span>Home</li>
		<li class="btn">Contribution</li>
		<li class="btn">Our Mission</li>
	</ul>
	<div>
		<p class="btn flex items-center gap-2 text-base/none font-semibold">
			<span>
				<svg width="22" height="23" viewBox="0 0 22 23" fill="none" xmlns="http://www.w3.org/2000/svg">
					<rect width="2.5" height="23" transform="translate(10)" fill="#1E1F1A"/>
					<rect width="2" height="23" transform="translate(19.3086 1.95605) rotate(45)" fill="#1E1F1A"/>
					<rect width="2" height="23" transform="translate(2 3.41406) rotate(-45)" fill="#1E1F1A"/>
					<circle cx="11" cy="11" r="3" fill="#1E1F1A"/>
					<rect width="22" height="2" transform="translate(0 10)" fill="#1E1F1A"/>
				</svg>
			</span>
			Atacama</p>
	</div>
	<ul class="flex items-center gap-2">
		<li class="btn">Problems</li>
		<li class="btn">Projects</li>
		<a class="rounded-full border border-gray-100 hover:bg-primary hover:border-primary bg-white px-5 flex h-12 items-center justify-center text-base/none font-medium" href="/">Contact Us</a>
	</ul>
</nav>

<style>
	.btn {
		background: var(--color-neutral-50);
		display: flex;
		height: 3rem;
		align-items: center;
		justify-items: center;
		padding-inline: 1.5rem;
		border-radius: 9rem;
		font-size: 1rem;
		line-height: 1;
		font-weight: 500;
		cursor: pointer;

		&:hover {
			background: #E6E6E6;
		}
	}
</style>
