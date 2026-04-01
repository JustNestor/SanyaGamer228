<script>
	import Sidebar from "./lib/SideBar.svelte";
	import AboutMe from "./lib/AboutMe.svelte";
	import Experience from "./lib/Experience.svelte";

	const skills = [
		"C++",
		"HTML/CSS",
		"JavaScript",
		"Python",

	];

	const experiences = [
		{
			label: "C++",
			description:
				"Вмію реалізовувати складних алгоритмів та структур даних. Досвід оптимізації коду, робота зі стандартами C++ та бібліотекою STL. Опанував синтаксис мови, роботу з пам'яттю та принципи ООП.",
		},
		{
			label: "Python",
			description:
				"Пишу прості скрипти для автоматизації роботи. Використовую Python, щоб швидко вирішувати задачі, де потрібно щось обчислити або перевірити дані.",
		},
		{
			label: "Розробка сайту",
			description:
				"Вмію створювати структуру сторінок та налаштовувати їхній зовнішній вигляд: кольори, шрифти та відступи. Роблю так, щоб сайт мав гарний вигляд на екрані.",
		},
	];
</script>

<div class="bg-gray-100 min-h-screen">
	<div class="container mx-auto py-8">
		<div class="grid grid-cols-4 sm:grid-cols-12 gap-6 px-4">
			<div class="col-span-4 sm:col-span-3">
				<Sidebar name="Кубик Олександр" title="Студент" {skills} />
			</div>

			<div class="col-span-4 sm:col-span-9">
				<div class="bg-white shadow rounded-lg p-6">
					<AboutMe title="Про мене">
						<p>
							Живу у Львові і навчаюсь в ЛНУ ім. Івана Франка на
							факультеті прикладної математики та інформатики.
							Цікавлюся програмуванням та різними видами спорту: 
							футбол, настільний теніс, волейбол.
						</p>
					</AboutMe>

					<Experience {experiences} />
				</div>
			</div>
		</div>
	</div>
</div>
