<script>
	import Sidebar from "./lib/SideBar.svelte";
	import AboutMe from "./lib/AboutMe.svelte";
	import Experience from "./lib/Experience.svelte";

	const skills = [
		"Rust",
		"Linux",
		"Vulkan",
		"Solana",
		"HTML/CSS/TS",
		"Svelte",
		"Tailwind CSS",
		"Python",
	];

	const experiences = [
		{
			label: "Вивчення Vulkan",
			description:
				"Почав вивчати Vulkan з ціллю створити свій ігровий двигун та гру на ньому. Для досягнення цієї цілі почав створення бібілотеки на Rust, яка ставить за мету абстрагувати Vulkan та зробити його використання більш приємним.",
		},
		{
			label: "Вивчення Solana",
			description:
				"Проходжу інтенсив Solana StartUp Terminal, який навчає, як розробляти рішення під блокчейн Solana.",
		},
		{
			label: "Розробка нового сайту факультету",
			description:
				"Відповідаю за створення системи для пошуку файлів на базі RAG.",
		},
	];
</script>

<div class="bg-gray-100 min-h-screen">
	<div class="container mx-auto py-8">
		<div class="grid grid-cols-4 sm:grid-cols-12 gap-6 px-4">
			<div class="col-span-4 sm:col-span-3">
				<Sidebar name="Комарницький Нестор" title="Студент" {skills} />
			</div>

			<div class="col-span-4 sm:col-span-9">
				<div class="bg-white shadow rounded-lg p-6">
					<AboutMe title="Про мене">
						<p>
							Живу у Львові і навчаюсь в ЛНУ ім. Івана Франка на
							факультеті електроніки та комп'ютерних технологій.
							Обожнюю читати та вивчати складні та водночас цікаві
							технології. Фанат Arch Linux та Rust.
						</p>
					</AboutMe>

					<Experience {experiences} />
				</div>
			</div>
		</div>
	</div>
</div>
