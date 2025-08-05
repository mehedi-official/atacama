<script lang="ts">
	import '../app.css';
	import {  } from "$lib/fonts/Gilroy-Regular.woff2";

	let { children } = $props();
</script>

{@render children()}


<style>
	:global(body) {
		font-family: 'Gilroy', sans-serif;
	}
	@font-face {
		font-family: 'Gilroy';
		src: local('Gilroy Regular'), local('Gilroy-Regular'),
			url('$lib/fonts/Gilroy-Regular.woff2') format('woff2');
		font-weight: normal;
		font-style: normal;
	}

	@font-face {
		font-family: 'Gilroy';
		src: local('Gilroy Medium'), local('Gilroy-Medium'),
			url('$lib/fonts/Gilroy-Medium.woff2') format('woff2');
		font-weight: 500;
		font-style: normal;
	}

	@font-face {
		font-family: 'Gilroy';
		src: local('Gilroy Semibold'), local('Gilroy-Semibold'),
			url('$lib/fonts/Gilroy-Semibold.woff2') format('woff2');
		font-weight: 600;
		font-style: normal;
	}
</style>
