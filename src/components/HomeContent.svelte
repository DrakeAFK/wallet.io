<script lang="ts">
	const mockdata = [
		{
			title: 'Extreme performance',
			description:
				'This dust is actually a powerful poison that will even make a pro wrestler sick, Regice cloaks itself with frigid air of -328 degrees Fahrenheit',
			icon: null
		},
		{
			title: 'Privacy focused',
			description:
				'People say it can run at the same speed as lightning striking, Its icy body is so cold, it will not melt even if it is immersed in magma',
			icon: null
		},
		{
			title: 'No third parties',
			description:
				'They’re popular, but they’re rare. Trainers who show them off recklessly may be targeted by thieves',
			icon: null
		}
	]
</script>

<div class="container mx-auto max-w-screen-lg px-10 py-16">
	<div class="text-center space-y-4">
		<span class="badge variant-filled-primary uppercase">Best Company Ever</span>
		<div class="text-xl md:text-3xl font-bold">
			Integrate effortlessly with any technology stack
		</div>
		<p
			class="max-w-xl opacity-60 mx-auto after:mx-auto after:mt-3 after:bg-primary-500 after:w-12 after:h-0.5 after:block"
		>
			Every once in a while, you’ll see a Golbat that’s missing some fangs. This happens when hunger
			drives it to try biting a Steel-type Pokémon.
		</p>
	</div>
	<div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4 pt-16">
		{#each mockdata as feature}
			<div class="card p-4 space-y-2">
				<svelte:component this={feature.icon} class="text-4xl text-primary-500" />
				<div class="font-bold after:mt-3 after:bg-primary-500 after:w-12 after:h-0.5 after:block">
					{feature.title}
				</div>
				<div class="text-xs opacity-60">
					{feature.description}
				</div>
			</div>
		{/each}
	</div>
</div>
