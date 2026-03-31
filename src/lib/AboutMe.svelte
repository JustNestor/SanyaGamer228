<script>
	export let title = "About Me";
</script>

<div class="mb-6">
	<h2 class="text-xl font-bold mb-4">{title}</h2>
	<div class="text-gray-700">
		<slot />
	</div>
</div>
