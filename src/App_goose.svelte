<script>
	import Sidebar from "./lib/SideBar.svelte";
	import AboutMe from "./lib/AboutMe.svelte";
	import Experience from "./lib/Experience.svelte";

	const skills = [
		"C#",
		"SQL",
		"git",
		"WPF",
		"HTML/CSS",
		"SCSS",
		"Docker",
		"Python",
	];

	const experiences = [
		{
			label: "Вивчення C#",
			description:
				"Почав вивчати C# на 1 курсі НТУ ДП, продовжую вивчати",
		},
		{
			label: "Вивчення SQL",
			description:
				"Почав вивчати SQL на 1 курсі НТУ ДП, продовжую вивчати",
		},
		{
			label: "Вивчення Docker",
			description:
				"Почав вивчати Docker на 1 курсі НТУ ДП, продовжую вивчати",
		},
	];
</script>

<div class="bg-gray-100 min-h-screen">
	<div class="container mx-auto py-8">
		<div class="grid grid-cols-4 sm:grid-cols-12 gap-6 px-4">
			<div class="col-span-4 sm:col-span-3">
				<Sidebar name="Гребенюк Кіріл Вікторович" title="Студент" {skills} />
			</div>

			<div class="col-span-4 sm:col-span-9">
				<div class="bg-white shadow rounded-lg p-6">
					<AboutMe title="Про мене">
						<p>
							Проживаю в с.Сергіївка Дніпропетровської області. Навчаюсь на 1 курсі НТУ ДП (Інженерія ПЗ), роблю проект OurHub
						</p>
					</AboutMe>

					<Experience {experiences} />
				</div>
			</div>
		</div>
	</div>
</div>
