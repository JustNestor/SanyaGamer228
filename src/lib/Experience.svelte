<script>
	export let experiences = [];
</script>

<div class="mt-6">
	<h2 class="text-xl font-bold mb-4">Досвід</h2>

	{#each experiences as exp}
		<div class="mb-6">
			<span class="text-gray-700 font-bold">{exp.label}</span>
			<p class="mt-2">{exp.description}</p>
		</div>
	{/each}
</div>
