<script>
    import svelteLogo from "./assets/svelte.svg";
    import viteLogo from "./assets/vite.svg";
    import heroImg from "./assets/hero.png";
    import Counter from "./lib/Counter.svelte";
    import "./app.css";
    import SideBar from "./lib/SideBar.svelte";
    import Main from "./lib/Main.svelte";
</script>

<div class="bg-gray-100">
    <div class="container mx-auto py-8">
        <div class="grid grid-cols-4 sm:grid-cols-12 gap-6 px-4">
            <SideBar name={"Nestor"} />
            <Main />
        </div>
    </div>
</div>
