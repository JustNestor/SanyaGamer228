<script>
	import Sidebar from "./lib/SideBar.svelte";
	import AboutMe from "./lib/AboutMe.svelte";
	import Experience from "./lib/Experience.svelte";

	const skills = [
		"JavaScript",
		"React",
		"Node.js",
		"HTML/CSS",
		"Tailwind CSS",
	];

	const experiences = [
		{
			label: "Web Developer",
			description:
				"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed finibus est vitae tortor ullamcorper, ut vestibulum velit convallis. Aenean posuere risus non velit egestas suscipit.",
		},
		{
			label: "Open Source Project",
			description:
				"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed finibus est vitae tortor ullamcorper, ut vestibulum velit convallis. Aenean posuere risus non velit egestas suscipit.",
		},
		{
			label: "Computer Science Degree",
			description:
				"Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed finibus est vitae tortor ullamcorper, ut vestibulum velit convallis. Aenean posuere risus non velit egestas suscipit.",
		},
	];
</script>

<div class="bg-gray-100 min-h-screen">
	<div class="container mx-auto py-8">
		<div class="grid grid-cols-4 sm:grid-cols-12 gap-6 px-4">
			<div class="col-span-4 sm:col-span-3">
				<Sidebar name="John Doe" title="Студент" {skills} />
			</div>

			<div class="col-span-4 sm:col-span-9">
				<div class="bg-white shadow rounded-lg p-6">
					<AboutMe title="Про мене">
						<p>
							Lorem ipsum dolor sit amet, consectetur adipiscing
							elit. Sed finibus est vitae tortor ullamcorper, ut
							vestibulum velit convallis. Aenean posuere risus non
							velit egestas suscipit. Nunc finibus vel ante id
							euismod. Vestibulum ante ipsum primis in faucibus
							orci luctus et ultrices posuere cubilia Curae;
							Aliquam erat volutpat. Nulla vulputate pharetra
							tellus, in luctus risus rhoncus id.
						</p>
					</AboutMe>

					<Experience {experiences} />
				</div>
			</div>
		</div>
	</div>
</div>
