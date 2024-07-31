<script>
    import Icon from '@iconify/svelte';
    import { onMount } from 'svelte';

    export let open = true

    let baseUrl =  '';
    onMount(() => {
        let currentPath = window.location.pathname;
        baseUrl = currentPath === '/impressum' ? '/' : '';
    });

    const finClick = () => {
        if (window.innerWidth <= 768) {
            open = false;
        }
    }
</script>

<aside class="absolute w-full h-full bg-gray-200 shadow-lg" class:open>
    <nav class="p-12 text-xl">
        <div class="logo-container">
            <img src="/favicon.png" alt="Stanic Logo" class="img-logo"/>
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
        <div class="spacer"></div>
        <button on:click={finClick} class="container">
            <a class="block" href="/">
                <Icon icon="material-symbols-light:home-rounded" />Hauptseite&nbsp;&nbsp;&nbsp;
            </a>
        </button>
        <button on:click={finClick} class="container">
            <a class="block" href={baseUrl + "#service"}>
                <Icon icon="material-symbols-light:account-tree-rounded" />Service&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            </a>
        </button>
        <button on:click={finClick} class="container">
            <a class="block" href={baseUrl + "#about"}>
                <Icon icon="material-symbols-light:person-pin-rounded" />Über mich&nbsp;&nbsp;&nbsp;
            </a>
        </button>
        <button on:click={finClick} class="container">
            <a class="block" href={baseUrl +"#kontakt"}>
                <Icon icon="material-symbols-light:phone-in-talk-rounded" />Kontakt&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
            </a>
        </button>
        <button on:click={finClick} class="container">
            <a class="block" href="/impressum">
                <Icon icon="icomoon-free:section"/>Impressum
            </a>
        </button>
    </nav>
</aside>

<style>
    aside {
        z-index: 50;
        position: fixed;
        background-color: #0e4072;
        width: 25%;
        left: 100%;
        transition: left 0.3s ease-in-out;
        justify-content: center;
    }
    @media (min-width: 768px) {
        aside {
            display: flex;
        }
    }
    @media (max-width: 768px) {
        aside {
            width: 100%;
        }
    }

    #name {
        font-size: 20px;
    }

    .open {
        left: 75%;
    }
    @media (max-width: 768px) {
        .open {
            left: 0;
        }
    }
    .logo-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
    }
    .img-logo {
        max-width: 260px;
    }
    .img-text {
        text-align: center;
        margin-top: 5px;
        font-size: 0.32cm;
        color: rgba(195, 223, 252, 0.8);
        line-height: 18px;
        font-weight: 400;
    }
    @media (max-width: 768px) {
        .img-text {
            font-size: 0.4cm;
        }
    }
    .img-logo{
        max-width: 160px;
    }
    .spacer {
        height: 25px;
    }
    .container {
        display: flex;
        font-size: 25px;
        margin-top: 15px;
        letter-spacing: -0.6px;
        justify-content: center;
    }
    .container :global(svg) {
        font-size: 35px;
        margin-right: 10px;
    }
    .block {
        display: flex;
        color:  aliceblue;
        align-items: center;
        text-align: center;
        transition: color 0.3s ease, background-color 0.3s ease;
        padding: 1px;

    }
    .block:hover {
        color: #aec8e3;
    }
    .p-12 {
        padding-top: 20px !important;
        padding-right: 25px !important;
        padding-left: 25px !important;
    }
</style>