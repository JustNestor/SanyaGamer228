<script>
	import Sidebar from "./lib/SideBar.svelte";
	import AboutMe from "./lib/AboutMe.svelte";
	import Experience from "./lib/Experience.svelte";

	const skills = [
		"C#",
		"SQL",
		"GitHub",
		"Figma",
		"Adobe Photoshop",
		"Adobe Illustrator",
	];

	const experiences = [
		{
			label: "Вивчення C#",
			description:
					"Почав вивчати C# під час навчання на першому курсі НТУ «Дніпровська політехніка». Наразі володію базовими навичками програмування цією мовою та продовжую її активне вивчення і вдосконалення.",
		},
		{
			label: "Вивчення SQL",
			description:
					"Почав опановувати SQL під час навчання на першому курсі НТУ «Дніпровська політехніка». Наразі маю базові навички роботи з базами даних та продовжую активно поглиблювати свої знання.",
		},
		{
			label: "Вивчення Adobe Photoshop",
			description:
					"Володію на високому рівні. Маю впевнені практичні навички роботи з програмою, які активно використовую для створення графічного дизайну, розробки UI/UX та підготовки ігрової графіки.",
		},
	];
</script>

<div class="bg-gray-100 min-h-screen">
	<div class="container mx-auto py-8">
		<div class="grid grid-cols-4 sm:grid-cols-12 gap-6 px-4">
			<div class="col-span-4 sm:col-span-3">
				<Sidebar name="Погорілий Михайло Олександрович" title="Студент" {skills} />
			</div>

			<div class="col-span-4 sm:col-span-9">
				<div class="bg-white shadow rounded-lg p-6">
					<AboutMe title="Про мене">
						<p>
							Студент 1-го курсу НТУ ДП («Інженерія програмного забезпечення») з м. Кривий Ріг. Маю сильний аналітичний та творчий бекграунд (закінчив математичний ліцей та художню школу з відзнаками ). Активно практикуюсь у GameDev-сфері. Впевнено володію Adobe Photoshop , маю досвід створення UI/UX  та продовжую активно вивчати інструменти розробки (C#, SQL, GitHub).
						</p>
					</AboutMe>

					<Experience {experiences} />
				</div>
			</div>
		</div>
	</div>
</div>