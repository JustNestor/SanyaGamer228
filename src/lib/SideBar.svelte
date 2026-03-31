<script>
	export let skills = [];
	export let name = "John Doe";
	export let title = "Software Developer";
</script>

<div class="bg-white shadow rounded-lg p-6">
	<div class="flex flex-col items-center">
		<h1 class="text-xl font-bold">{name}</h1>
		<p class="text-gray-700">{title}</p>
	</div>

	<hr class="my-6 border-t border-gray-300" />

	<div class="flex flex-col">
		<span class="text-gray-700 uppercase font-bold tracking-wider mb-2"
			>Skills</span
		>
		<ul>
			{#each skills as skill}
				<li class="mb-2">{skill}</li>
			{/each}
		</ul>
	</div>
</div>
