<script>
	import '../app.css';
	import Header from '../components/Header.svelte';
	import Footer from '../components/Footer.svelte';
	let y;
	let innerHeight;
	let innerWidth;
	function goTop() {
		document.body.scrollIntoView();
	}
</script>

<div
	class="relative flex flex-col z-30 max-w-[1400px] mx-auto w-full text-sm sm:text-base min-h-screen"
>
	<div
		class={'fixed bottom-0 w-full duration-200 p-10 z-[10]' +
			(y > 0 ? ' opacity-full pointer-events-auto' : ' opacity-0 pointer-events-none')}
	>
		<button on:click={goTop} class="ml-auto text-violet-400 px-3 sm:px-4 cursor-pointer">
			<i class="fa-solid fa-arrow-up grid place-items-center aspect-square"></i>
		</button>
	</div>
	<Header {y} />
	<slot />
	<Footer />
</div>

<svelte:window bind:scrollY={y} bind:innerHeight bind:innerWidth />
