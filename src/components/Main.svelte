<script>
	import Step from './Step.svelte';
	let steps = [
		{ name: 'Wordly', icon: 'fa-solid fa-list' },
		{ name: 'Wordly Github', icon: 'fa-solid fa-code-branch' },
		{ name: 'Wordly Github', icon: 'fa-solid fa-code-branch' }
	];
</script>

<main class="flex flex-col flex-1 p-4">
	<section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">
		<div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">
			<h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
				Hi! I'm <span class="poppins text-violet-400">Phil</span> Webb <br />Full Stack
				<span class="poppins text-violet-400">Developer</span>
			</h2>
			<p class="text-base sm:text-lg md:text-xl">
				My <span class="text-violet-400">favourite tech</span> includes JavaScript, TypeScript, React,
				Svelte, Node.js, Express, MongoDB, PostgreSQL, and GraphQL.
			</p>
			<!-- svelte-ignore a11y-invalid-attribute -->
			<a
				href="#"
				target="_blank"
				class="blueShadow mx-auto lg:mr-auto text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
			>
				<div
					class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
				></div>
				<h4 class="relative z-9">Get in touch &rarr;</h4>
			</a>
		</div>
		<div class="relative shadow-2xl grid place-items-center rounded-full">
			<img
				src={'images/profile.jpeg'}
				class="rounded-full object-cover z-[2] max-h=[70vh]"
				alt=""
			/>
		</div>
	</section>
	<section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">
		<div class="flex flex-col gap-2 text-center">
			<h6 ckass="text-lg sm:text-xl md:text-2xl">A few of my creative endeavours</h6>
			<h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
				Curious to <span class="poppins text-violet-400">see</span> my work?
			</h3>
		</div>
		<a
			href="https://philrwebb-word.netlify.com"
			target="_blank"
			class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
			>A Svelte wordle Clone</a
		>
		<div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
			<Step step={steps[0]}>
				<p>
					This is a Wordle Clone written in Svelte and hosted at netlify. Fullstack app that uses
					supabase to store the list of words.
				</p>
				<strong class="text-violet-400">Svelte and Supabase</strong>
			</Step>
			<Step step={steps[1]}>
				<p>This is the Github repo for the Wordle Clone.</p>
				<strong class="text-violet-400">Svelte and Supabase</strong>
			</Step>
			<Step step={steps[2]}></Step>
		</div>
	</section>
	<section
		id="about"
		class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gam-20 md:gap-24 relative"
	>
		<div
			class="flex flex-col gap-2 text-center relative before:relative before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:relative after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700"
		>
	<h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6></div>f
	</section>
</main>
