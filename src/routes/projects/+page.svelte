<script>
	import Step from '../../components/Step.svelte';
	let steps = [
		{
			name: 'Smoljames Store',
			icon: 'fa-solid fa-cart-shopping',
			description:
				'Smoljames Store is a a merchanising store created with Next.js, Commerce.js & Stripe! Commerce.js is a CMS for managing project and Stripe is used for all transaction handling.'
		},
		{
			name: 'Utlimate Todos',
			icon: 'fa-solid fa-list-check',
			description:
				'Test for model robustness with customized test profiles and receive exhaustive reporting on the performance and potential vulnerabilities of your model.'
		},
		{
			name: 'Pokédex',
			icon: 'fa-solid fa-diagram-project',
			description:
				'Augment your datasets with our filters and dataset manipulations to ensure your models are trained on the highest quality datasets (coming soon).'
		}
	];
</script>

<section class=" flex flex-col gap-24 h-screen" id="projects">
	<div class="flex flex-col gap-2 text-center">
		<h6 class="text-large sm:text-xl md:text-3xl">
			A few of my <span class="text-violet-400 poppins">creative</span> endeavors! 🔥
		</h6>
	</div>

	<div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
		<Step step={steps[0]}>
			<p>
				Smoljames Store is a a merchanising store created with <strong class="text-violet-400"
					>Next.js, Commerce.js, Stripe & Node.js + Express.js!</strong
				> Commerce.js is a product CMS and Stripe is used for all transaction handling.
			</p>
		</Step>
		<Step step={steps[1]}>
			<p>
				Ultimate Todos is a Full Stack <strong class="text-violet-400">Next.js</strong>,
				<strong class="text-violet-400">Node.js + Express.js</strong>
				& <strong class="text-violet-400">Firebase</strong> CRUD application that allows a user to login,
				manage a tidy and efficacious todo list, and persist this information across devices.
			</p>
		</Step>
		<Step step={steps[2]}>
			<p>
				The Pokédex is a <strong class="text-violet-400">SvelteKit & TailwindCSS</strong>
				web application, hosted on
				<strong class="text-violet-400">Netlify</strong>, that consumes and caches the
				<strong class="text-violet-400">Pokémon API</strong>
				to display all Pokémon information. Gotta catch them all!
			</p>
		</Step>
	</div>
</section>
