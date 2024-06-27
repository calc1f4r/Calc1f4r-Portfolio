<script>
	export let imgSrc = '';
	export let title = '';
	export let description = '';
	export let liveWebsiteUrl = '';
	export let githubRepoUrl = '';
	export let youtubeLink = '';
</script>

<div
	class="card cursor-crosshair max-w-md mx-auto border bg-red-300/10 border-red-300 p-4 rounded-lg overflow-hidden shadow-md hover:shadow-lg transition-all duration-300 ease-in-out"
>
	<div class="image-container aspect-w-16 aspect-h-9 w-full overflow-hidden rounded-lg">
		<img
			src={imgSrc}
			alt={title}
			class="w-full h-full object-cover transition duration-300 ease-in-out hover:scale-105"
		/>
	</div>
	<div class="content pt-4 flex flex-col justify-center gap-2">
		<h2
			class="text-xl font-semibold text-red-300 hover:text-red-400 transition-colors duration-300"
		>
			{title}
		</h2>
		<p class="text-base text-red-100">{description}</p>
	</div>
	<div class="actions flex justify-between mt-8 align-self-end justify-self-end">
		{#if liveWebsiteUrl}
			<a
				href={liveWebsiteUrl}
				target="_blank"
				class="inline-flex items-center mt-3 text-red-300 transition duration-300 hover:text-red-400"
				aria-label="Visit Website"
			>
				<i class="fas fa-globe mr-2"></i> Visit Website
			</a>
		{/if}
		<div class="flex items-center">
			{#if githubRepoUrl}
				<a
					href={githubRepoUrl}
					target="_blank"
					class="text-white hover:text-black/100 transition duration-300"
					aria-label="GitHub Repository"
				>
					<i class="fab fa-github mr-2"></i>
				</a>
			{/if}
			{#if youtubeLink}
				<a
					href={youtubeLink}
					target="_blank"
					class="text-white hover:text-red-600 transition duration-300"
					aria-label="YouTube Video"
				>
					<i class="fab fa-youtube ml-4"></i>
				</a>
			{/if}
		</div>
	</div>
</div>

<style>
	.card {
		width: 100%; /* Use max-width for maximum size, e.g., max-width: 320px; */
		display: flex;
		flex-direction: column;
	}
	.image-container img {
		aspect-ratio: 16 / 9;
	}
	.content {
		flex: 1; /* Ensures that the content section expands to fill available space, pushing actions to the bottom */
		display: flex;
		flex-direction: column;
	}
	.actions {
		margin-top: auto; /* Pushes actions to the bottom */
	}
</style>
