<script>
    import Icon from '@iconify/svelte';

    export let open = true
</script>
<aside class="absolute w-full h-full bg-gray-200 border-r-2 shadow-lg" class:open>
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
        <div class="container">
            <a class="block" href="/">
                <Icon icon="material-symbols-light:home" style="font-size: 30px; margin-right: 10px;"/>Hauptseite
            </a>
        </div>
        <div class="container">
            <a class="block" href="#service">
                <Icon icon="material-symbols-light:account-tree" style="font-size: 30px; margin-right: 10px;"/>Service
            </a>
        </div>
        <div class="container">
            <a class="block" href="#about">
                <Icon icon="material-symbols-light:frame-person-sharp" style="font-size: 30px; margin-right: 10px;"/>Über mich
            </a>
        </div>
        <div class="container">
            <a class="block" href="#kontakt">
                <Icon icon="material-symbols-light:perm-phone-msg-sharp" style="font-size: 30px; margin-right: 10px;"/>Kontakt
            </a>
        </div>
        <div class="container">
            <a class="block" href="/impressum">
                <Icon icon="icomoon-free:section" style="font-size: 30px; margin-right: 10px;"/>Impressum
            </a>
        </div>
    </nav>
</aside>

<style>
    .container {
        display: flex;
        font-size: 20px;
        margin-top: 15px;
    }
    .block{
        display: flex;
        color:  aliceblue;
        align-items: center;
        text-align: left;
        transition: color 0.3s ease, background-color 0.3s ease;
        padding: 1px;
    }
    .block:hover {
        color: #aec8e3;
    }
    aside {
        z-index: 50;
        position: fixed;
        background-color: #356ba2;
        width: 25%;
        left: 100%;
        transition: left 0.3s ease-in-out
    }

    .open {
        left: 75%;
    }
    .img-text {
        text-align: center;
        margin-top: 10px;
        font-size: 0.32cm;
        color:  aliceblue;
        line-height: 15px;
    }
    .img-logo {
        max-width: 240px;
    }
    .logo-container {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
    }
    .spacer {
        height: 20px;
    }
    @media (max-width: 768px) {
        aside {
            width: 100%;
        }

        .open {
            left: 0;
        }
        .img-text {
            font-size: 0.4cm;
        }
        .img-logo{
            max-width: 160px;
        }
        .container{
            justify-content: space-around;
        }
    }
</style>