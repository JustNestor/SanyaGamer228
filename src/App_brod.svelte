<script>
	import Sidebar from "./lib/SideBar.svelte";
	import AboutMe from "./lib/AboutMe.svelte";
	import Experience from "./lib/Experience.svelte";

	const skills = ["SQL", "Python", "C#", "HTML/CSS"];

	const experiences = [
		{
			label: "Створюю базу даних для своєї курсової роботи ",
			description:
				"Створюю базу даних для оподаткування земельних ділянок.",
		},
		{
			label: "Проходжу курси по HTML/CSS",
			description: "Збільшую свої загальні знання.",
		},
		{
			label: "Вивчаю С#",
			description:
				"Вивчаю свою першу мову програмування C#, сподіваюсь отримати фундаментальні знання.",
		},
	];
</script>

<div class="bg-gray-100 min-h-screen">
	<div class="container mx-auto py-8">
		<div class="grid grid-cols-4 sm:grid-cols-12 gap-6 px-4">
			<div class="col-span-4 sm:col-span-3">
				<Sidebar name="Євген Пелих" title="Студент" {skills} />
			</div>

			<div class="col-span-4 sm:col-span-9">
				<div class="bg-white shadow rounded-lg p-6">
					<AboutMe title="Про мене">
						<p>
							Привіт! Я студент, який захоплюється програмуванням
							та базами даних. Маю досвід у SQL, Python, C#, а
							також в HTML/CSS. Моя мета - розвиватися в галузі
							інформаційних технологій та створювати корисні
							проекти. У вільний час я люблю вивчати нові
							технології, працювати над власними проектами та
							спілкуватися з іншими ентузіастами програмування. Я
							завжди відкритий до нових можливостей та готовий
							вчитися, щоб досягти своїх цілей у світі IT.
						</p>
					</AboutMe>

					<Experience {experiences} />
				</div>
			</div>
		</div>
	</div>
</div>
