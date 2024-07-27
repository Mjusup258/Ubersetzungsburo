<script>
    import Icon from '@iconify/svelte';
    export let open = true
</script>

<aside class="absolute w-full h-full bg-gray-200 border-r-2 shadow-lg" class:open>
    <nav class="p-12 text-xl">
        <img src="./static/favicon.png"/>
        <a class="block" href="#main"><Icon icon="material-symbols-light:home" />Hauptseite</a>
        <a class="block" href="#service"><Icon icon="material-symbols-light:account-tree" />Service</a>
        <a class="block" href="#about"><Icon icon="material-symbols-light:frame-person-sharp" />Über mich</a>
        <a class="block" href="#kontakt"><Icon icon="material-symbols-light:perm-phone-msg-sharp" />Kontakt</a>
        <a class="block" href="#impressum"><Icon icon="icomoon-free:section" />Impressum</a>
    </nav>
</aside>

<style>
    aside {
        width: 25%;
        left: 100%;
        transition: left 0.3s ease-in-out
    }

    .open {
        left: 75%;
    }
    @media (max-width: 768px) {
        aside {
            width: 100%;
        }

        .open {
            left: 0;
        }
    }
</style>