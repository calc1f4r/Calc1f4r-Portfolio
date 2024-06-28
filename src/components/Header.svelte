<script>
	export let y;
	let tabs = [
		{ name: 'Home', link: '/' },
		{ name: 'About', link: '/about' },
		{ name: 'Projects', link: '/projects' },
		{ name: 'Writings', link: '/blog' }
	];
	import { page } from '$app/stores';
	$: currentPath = $page.url.pathname;
	let menuOpen = false;

	function toggleMenu() {
		menuOpen = !menuOpen;
	}
</script>

<header
	class={'sticky z-[10] top-0 duration-200 px-6 flex items-center justify-between border border-solid ' +
		(y > 0 ? 'py-4 bg-slate-950 border-violet-950' : 'py-6 bg-transparent border-transparent')}
>
	<h1 class="font-medium">
		<b class="poppins"><a href="/">Yash | calc1f4r</a></b>
	</h1>
	<nav class="hidden sm:flex items-center gap-4">
		{#each tabs as tab, index}
			<a
				href={tab.link}
				aria-current={currentPath === tab.link ? 'page' : undefined}
				class="duration-200 font-medium hover:text-violet-400 {currentPath === tab.link
					? 'text-violet-400'
					: ''}"
			>
				<p>{tab.name}</p>
			</a>
		{/each}
	</nav>
	<div class="sm:hidden flex items-center">
		<button
			class="text-white focus:outline-none"
			on:click={toggleMenu}
			aria-label="Toggle navigation"
		>
			{#if menuOpen}
				<svg
					class="w-6 h-6"
					fill="none"
					stroke="currentColor"
					viewBox="0 0 24 24"
					xmlns="http://www.w3.org/2000/svg"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M6 18L18 6M6 6l12 12"
					></path>
				</svg>
			{:else}
				<svg
					class="w-6 h-6"
					fill="none"
					stroke="currentColor"
					viewBox="0 0 24 24"
					xmlns="http://www.w3.org/2000/svg"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M4 6h16M4 12h16m-7 6h7"
					></path>
				</svg>
			{/if}
		</button>
	</div>
	{#if !menuOpen}
		<a
			href="https://x.com/calc1f4r"
			target="_blank"
			class="blueShadow relative overflow-hidden px-5 py-2 group rounded-full bg-white text-slate-950 hidden sm:block"
		>
			<div
				class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full duration-200"
			></div>
			<h4 class="relative z-9">Get in touch</h4>
		</a>
	{/if}
</header>
{#if menuOpen}
	<nav class="sm:hidden flex flex-col items-start px-6 py-4 bg-slate-950 text-white space-y-4">
		{#each tabs as tab, index}
			<a
				href={tab.link}
				aria-current={currentPath === tab.link ? 'page' : undefined}
				class="duration-200 font-medium hover:text-violet-400 {currentPath === tab.link
					? 'text-violet-400'
					: ''}"
				on:click={() => (menuOpen = false)}
			>
				<p>{tab.name}</p>
			</a>
		{/each}
	</nav>
{/if}

<style>
	.active-link {
		color: #7c3aed; /* Violet color */
	}
	.blueShadow {
		box-shadow: 0 4px 14px rgba(0, 0, 0, 0.1);
	}
	.blueShadow:hover {
		box-shadow: 0 6px 20px rgba(0, 0, 0, 0.15);
	}
</style>
