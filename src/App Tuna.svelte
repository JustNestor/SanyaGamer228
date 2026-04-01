<script>
    import Sidebar from "./lib/SideBar.svelte";
    import AboutMe from "./lib/AboutMe.svelte";
    import Experience from "./lib/Experience.svelte";

    const skills = [
        "Python",
        "Unity/C#",
        "HTML/CSS/JavaScript",
        "Основи OpenClaw",
        "Основи Arduino",
        "Основи проектування електронних схем",
        "Створення баз даних Firebase",
        "Базові команди Bash"
        
    ];

    const experiences = [
        {
            label: "Python",
            description:
                "Маю досвід використання Python у багатьох типах проектів. Таких як: автоматизація Telegram за допомогою pytelegrambotapi та Aiogram, веб-автоматизація з selenium, розробка ігор з Pygame, Ursina та Panda3D, а також парсинг HTML-сторінок за допомогою Pyparsing. Також маю досвід створення та управління базами даних за допомогою SQLite.",
        },
        {
            label: "Unity/C#",
            description:
                "Мав досвід розробки 2D та 3D ігор на Unity, включаючи підключення гри до бази даних, створеної за допомогою Firebase"
                },
        {
            label: "Основи схемотехніки",
            description:
                "Маю досвід створення базових електронних схем у Multisim, а також їх реалізації з використанням фізичних плат та елементів.",
        },
    ];
</script>

<div class="bg-gray-100 min-h-screen">
    <div class="container mx-auto py-8">
        <div class="grid grid-cols-4 sm:grid-cols-12 gap-6 px-4">
            <div class="col-span-4 sm:col-span-3">
                <Sidebar name="Дідух Святослав" title="Студент" {skills} />
            </div>

            <div class="col-span-4 sm:col-span-9">
                <div class="bg-white shadow rounded-lg p-6">
                    <AboutMe title="Про мене">
                        <p>
                            Я живу у Львові та навчаюся у Львівському національному університеті імені Івана Франка на ФЕКТ. Люблю шахи та музику. Цікавлюся вбудованими системами, а також розробкою ігор.
                            Я великий шанувальник Linux.
                        </p>
                    </AboutMe>

                    <Experience {experiences} />
                </div>
            </div>
        </div>
    </div>
</div>