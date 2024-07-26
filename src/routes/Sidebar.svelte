<script>
    export let open = true
</script>

<aside class="absolute w-full h-full bg-gray-200 border-r-2 shadow-lg" class:open>
    <nav class="p-12 text-xl">
        <a class="block" href="#main">Hauptseite</a>
        <a class="block" href="#service">Service</a>
        <a class="block" href="#about">Über mich</a>
        <a class="block" href="#kontakt">Kontakt</a>
        <a class="block" href="#impressum">Impressum</a>
    </nav>
</aside>

<style>
    aside {
        left: 100%;
        transition: left 0.3s ease-in-out
    }

    .open {
        left: 0
    }
</style>