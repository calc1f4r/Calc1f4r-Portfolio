<script>
	export let imgSrc = '';
	export let title = '';
	export let description = '';
	export let githubRepoUrl = '';
	export let blogLink = '';
	export let playBackLink = '';
</script>

<div
	class="card cursor-crosshair max-w-md mx-auto border bg-green-300/10 border-green-300 p-4 rounded-lg overflow-hidden shadow-md hover:shadow-lg transition-all duration-300 ease-in-out"
>
	{#if imgSrc}
		<div class="image-container aspect-w-16 aspect-h-9 w-full overflow-hidden rounded-lg">
			<img
				src={imgSrc}
				alt={title}
				class="w-full h-full object-cover transition duration-300 ease-in-out hover:scale-105"
			/>
		</div>
	{/if}
	{#if playBackLink}
		<iframe
			src={playBackLink}
			{title}
			width="100%"
			height="250"
			frameborder="0"
			allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
			referrerpolicy="strict-origin-when-cross-origin"
			allowfullscreen
		></iframe>
	{/if}

	<div class="content pt-4 flex flex-col justify-center gap-2">
		<h2
			class="text-xl font-semibold text-green-300 hover:text-green-400 transition-colors duration-300"
		>
			{title}
		</h2>
		<p class="text-base text-green-100">{description}</p>
	</div>
	<div class="actions mt-8">
		<div class="flex items-center mt-3 gap-3">
			{#if githubRepoUrl}
				<a
					href={githubRepoUrl}
					target="_blank"
					class="text-white hover:text-black/100 transition duration-300"
					aria-label="GitHub Repository"
				>
					<i class="fab fa-github"></i>
				</a>
			{/if}
			{#if blogLink}
				<a
					href={blogLink}
					target="_blank"
					class="hover:text-green-300 transition duration-300"
					aria-label="Blog Link"
				>
					<i class="fa-solid fa-blog"></i>
				</a>
			{/if}
		</div>
	</div>
</div>

<style>
	.card {
		width: 100%;
		display: flex;
		flex-direction: column;
	}
	.image-container img {
		aspect-ratio: 16 / 9;
	}
	.content {
		flex: 1;
		display: flex;
		flex-direction: column;
	}
	.actions {
		margin-top: auto;
	}
</style>
