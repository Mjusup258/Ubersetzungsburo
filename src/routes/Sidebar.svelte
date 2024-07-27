<script>
    import Icon from '@iconify/svelte';
    export let open = true
</script>
<aside class="absolute w-full h-full bg-gray-200 border-r-2 shadow-lg" class:open>
    <nav class="p-12 text-xl">
        <div class="logo-container">
            <img src="./static/favicon.png" alt="Stanic Logo" class="img-logo"/>
            <div class="img-text">
                <b id="name">Vlado Stanić</b><br>
                Staatlich geprüfter Übersetzer für die <br>
                bosnische, kroatische und serbische Sprache <br>
                Friedenstr. 16, D-90765 Fürth <br>
                vlado.stanic@vodafonemail.de <br>
                Tel: +49 911 89293933 <br>
                Fax: +49 911 25356400 <br>
                Mob: +49 171 2971506
            </div>
        </div>
        <a class="nav-link" href="#main">
            <Icon class="icon" icon="material-symbols-light:home" />Hauptseite
        </a>
        <a class="nav-link" href="#service">
            <Icon class="icon" icon="material-symbols-light:account-tree" />Service
        </a>
        <a class="nav-link" href="#about">
            <Icon class="icon" icon="material-symbols-light:frame-person-sharp" />Über mich
        </a>
        <a class="nav-link" href="#kontakt">
            <Icon class="icon" icon="material-symbols-light:perm-phone-msg-sharp" />Kontakt
        </a>
        <a class="nav-link" href="#impressum">
            <Icon class="icon" icon="icomoon-free:section" />Impressum
        </a>
    </nav>
</aside>

<style>
/* Additional CSS for aligning icon and text */
.nav-link {
    display: flex;
    align-items: center;
}

.nav-link .icon {
    margin-right: 8px; /* Adjust spacing as needed */
}

/* Existing styles */
aside {
    width: 25%;
    left: 100%;
    transition: left 0.3s ease-in-out;
}

.open {
    left: 75%;
}

.img-text {
    text-align: center;
    margin-top: 10px;
    font-size: 0.32cm;
    color: black;
    line-height: 15px;
}

.logo-container {
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
}

@media (max-width: 768px) {
    aside {
        width: 100%;
    }

    .open {
        left: 0;
    }

    .img-text {
        font-size: 0.4cm; /* Increase font size for mobile devices */
    }

    .img-logo {
        max-width: 200px;
    }
}
</style>