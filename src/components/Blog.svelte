<script>
	export let title, link, image;
</script>

<a href={link} class="block hover:no-underline">
	<div
		class="card transition duration-300 ease-in-out transform hover:-translate-y-1 hover:shadow-xl bg-gray-800 border border-gray-700 rounded-lg overflow-hidden p-5 min-w-[300px] min-h-[350px]"
	>
		<div class="aspect-w-16 aspect-h-9 w-full overflow-hidden rounded-lg">
			<img
				src={image}
				alt={title}
				class="w-full h-full object-cover transition duration-300 ease-in-out hover:scale-105"
			/>
		</div>
		<div class="pt-4">
			<h2
				class="text-xl font-semibold text-gray-100 hover:text-violet-400 transition-colors duration-300"
			>
				{title}
			</h2>
		</div>
	</div>
</a>

<style>
	.card {
		transition:
			transform 0.3s ease,
			box-shadow 0.3s ease;
		background: rgba(255, 255, 255, 0.05);
	}
	.card:hover {
		transform: translateY(-5px);
	}
	a:hover {
		text-decoration: none;
	}
</style>
