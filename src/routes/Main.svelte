<script>
    import Icon from '@iconify/svelte';

</script>
<body>

    <main>
        <div class="title-section image">
            <div class="container">
                <div class="item">
                    <div class="bg-blue-transparent logo-fa">Ubersetzungsbüro<br>Vlado Stanić</div>
                    <div class="bg-blue-transparent simple">
                        <p>
                            <b>Vereidigte Übersetzer für die</b>
                            <br>
                            <b>bosnische, kroatische und serbische Sprache.</b></p></div>

                </div>
            </div>
        </div>

        <section class="service-section">
            <div class="container">
                <div class="row">
                    <div class="item col-md-4">
                        <div class="tm-work-item-inner">
                            <div class="service-icn"><Icon icon="material-symbols-light:bookmark-star-sharp" /></div>
                            <h3>Kompetenz und Professionalität</h3>
                            <p><b>Alle Texte werden sorgfältig übersetzt und mehrfach geprüft, um ein perfektes Ergebnis zu erzielen.</b></p>
                        </div>
                    </div>
                    <div class="item col-md-4 one">
                        <div class="tm-work-item-inner">
                            <div class="service-icn"><Icon icon="material-symbols-light:order-approve-sharp" /></div>
                            <h3>Qualitätssicherung</h3>
                            <p><b>Die Vergütung richtet sich nach dem Justizvergütungs- und Entschädigungsgesetz (JVEG). Selbstverständlich behandle ich alle Aufträge vertraulich.</b></p>
                        </div>
                    </div>
                    <div class="item col-md-4 two">
                        <div class="tm-work-item-inner">
                            <div class="service-icn"><Icon icon="material-symbols-light:content-paste-search-sharp" /></div>
                            <h3>Individuelle Lösungen</h3>
                            <p><b>Persönlicher Service: <br>Ihre Wünsche stehen im Mittelpunkt.</b> </p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section class="about-me-section" data-image-src="/Stack of books.jpg" id="About me">
            <div class="container">
                <div class="title text-left">
                    <h2>Über mich</h2>
                </div>
                <div class="col-lg-4 col-md-6 mb-4 contact-details">
                    <div class="tm-work-item-inner">
                        <p></p>
                        <ul class="tm-work-item-inner">
                            <li>
                                <p><b>Staatlich geprüfter, öffentlich bestellter und beeidigter Übersetzer für die bosnische, kroatische und serbische Sprache.</b></p>
                            </li>
                            <li>
                               <p><b>Maschinenbauingenieur Uni Zagreb - Konstrukteur im Bereich der Telekommunikation.</b></p>
                            </li>
                            <li>
                                <p><b>Tennislehrer / C-Lizenz / <br>Bayerischer Tennis-Verband</b></p>
                            </li>
                        </ul>
                    </div>
                </div>

            </div>
        </section>

        <section class="contact-section" id="Contact">
            <div class="container">
                <div class="title">
                    <h3>Kontaktieren Sie mich</h3>
                </div>
                <div class="row">
                    <!--
                    <div class="col-lg-5 col-md-6 mb-4 contact-form">
                        <div class="form tm-contact-item-inner">
                            <form action="#" method="POST">
                                <div class="form-group">
                                    <input name="name" type="text" class="form-control" placeholder="Name">
                                </div>
                                <div class="form-group">
                                    <input name="email" type="text" class="form-control" placeholder="E-Mail">
                                </div>
                                <div class="form-group">
                                    <textarea name="message" class="textarea form-control" placeholder="Nachricht"></textarea>
                                </div>
                                <div class="form-group text-right">
                                    <input type="submit" class="btn btn-primary" value="ABSENDEN">
                                </div>
                            </form>
                        </div>
                    </div>-->
                    <div class="col-lg-4 col-md-6 mb-4 contact-details">
                        <div class="tm-contact-item-inner-2">
                            <p><b>Haben Sie Fragen?  <br> Ich stehe Ihnen gerne zur Verfügung.</b></p>
                            <ul class="font-weight-light">
                                <li>
                                    <span class="icn"><Icon icon="material-symbols-light:deskphone-sharp" /></span>
                                    <span class="lbl">Tel:</span> <a href="+49 171 2971506">+49 911 89293933</a>
                                </li>
                                <li>
                                    <span class="icn"><Icon icon="material-symbols-light:fax-sharp" /></span>
                                    <span class="lbl">Fax:</span> <a href="+49 171 2971506">+49 911 25356400</a>
                                </li>
                                <li>
                                    <span class="icn"><Icon icon="material-symbols-light:phone-iphone-sharp" /></span>
                                    <span class="lbl">Mob:</span> <a href="+49 171 2971506">+49 171 2971506</a>
                                </li>
                                <br>
                                <li>
                                    <span class="icn"><Icon icon="material-symbols-light:stacked-email-sharp" /></span>
                                    <span class="lbl">Email:</span> <a href="vlado.stanic@vodafonemail.de">vlado.stanic@vodafonemail.de</a>
                                </li>
                                <li>
                                    <span class="icn"><Icon icon="material-symbols-light:globe" /></span>
                                    <span class="lbl">URL:</span> <a href="www.vladostanic.de">www.vladostanic.de</a>
                                </li>
                                <li>
                                    <span class="icn"><Icon icon="material-symbols-light:location-on" /></span>
                                    <span class="lbl">Ort:</span> <a href="https://maps.app.goo.gl/RLtDzeDvMFikXjkx5">Friedenstr. 16, 90765 Fürth</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <br>
                    <div class="col-lg-3 col-md-12 map">
                        <!-- Map
                        <div class="map-outer tm-mb-40">
                            <div class="gmap-canvas">
                                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2592.1452373619713!2d10.993142677563224!3d49.48176345663477!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x479f55ece582f7f7%3A0xb86e5d643998b3a2!2sFriedenstra%C3%9Fe%2016%2C%2090765%20F%C3%BCrth!5e0!3m2!1sen!2sde!4v1721639882849!5m2!1sen!2sde" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                            </div>
                        </div>
                    -->
                    </div>
                </div>
            </div>
        </section>

    </main>
</body>

<style>
    .title-section {
        position: relative;
        text-align: center;
        background-color: #99ccff;
        padding-top: 121px;
        align-items: flex-start;
    }

    .bg-blue-transparent {
        background-color: rgb(102 153 204 / 0.8);
    }

    .title-section .logo-fa {
        color: #fff;
        max-width: 400px;
        margin-bottom: 60px;
        margin-left: 50px;
        padding-top: 43px;
        padding-bottom: 35px;
        font-size: 40px;
        font-family: "Roboto Light",serif;
    }

    @media (max-width: 991px) {
        .title-section .logo-fa { margin: 0 auto 30px; }
    }

    @media (max-width: 767px) {
        .title-section .logo-fa {
            font-size: 28px;
            padding-top: 20px;
            padding-bottom: 15px;
        }
    }

    .title-section .simple {
        color: #fff;
        display: inline-block;
        margin: auto;
        margin-left: 97px;
        padding: 33px 68px 34px 68px;
        font-family: Verdana,serif;
    }

    @media (max-width: 991px) {
        .title-section .simple { margin-left: 0; }
    }

    @media (max-width: 767px) {
        .title-section .simple { padding: 16px 34px 17px 34px; }
    }

    .title-section .simple p {
        margin-bottom: 0;
        font-size: 22px;
    }

    @media (max-width: 991px) {
        .title-section .simple p { font-size: 20px; }
    }

    @media (max-width: 575px) {
        .title-section .simple p { font-size: 18px; }
    }
    .image {
        background-image: url("/section-1-bg.jpg");
        height: 100vh;
        width: 100%;
        display: flex;
        align-items: center;
        opacity: 0.8;
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        background-attachment: fixed;
    }

    /* <<< Service section (formerly known as work-section) >>> */

    .service-section {
        padding-top: 90px!important;
        padding-bottom: 90px!important;
        min-height: 850px;
        background-color: #6699cc;
    }
    .service-section .container {
        max-width: 1242px;
    }

    .tm-work-item-inner {
        max-width: 360px;
        margin-left: auto;
        margin-right: auto;
        margin-bottom: 30px;
    }
    @media (max-width: 767px) {
        .service-section .item {
            text-align: center;
            margin-bottom: 30px;
        }
    }


    .service-section .item.one {
        margin-top: 80px;
    }
    @media (max-width: 767px) {
        .service-section .item.one { margin-top: 0;}
    }

    .service-section .item.two {
        margin-top: 80px;
    }

    @media (max-width: 767px) {
        .service-section .item.two { margin-top: 0; }
    }


    .service-section .item .service-icn {
        width: 119px;
        height: 119px;
        display: block;
        border: 1px solid #fff;
        border-radius: 100%;
        color: #fff;
        font-size: 82px;
        display: -webkit-box;
        display: -ms-flexbox;
        display: flex;
        -webkit-box-pack: center;
        -ms-flex-pack: center;
        justify-content: center;
        -webkit-box-align: center;
        -ms-flex-align: center;
        align-items: center;
        text-transform: uppercase;
        margin-bottom: 30px;

    }

    .service-icn {
        margin: 0 auto 20px;
        max-width: 767px;
    }

    .service-section .item h3 {
        color: #111844;
        text-transform: uppercase;
        font-size: 27px;
        margin-bottom: 9px;

    }
    .service-section .item p {
        color: #fff;
        line-height: 31px;
        margin-bottom: 0;
        font-weight: lighter;
    }

    .service-section .item p {
        color: #fff;
        line-height: 31px;
        margin-bottom: 0;
    }
    .service-section .title h2 {
        color: #fff;
        font-size: 32px;
        margin-bottom: 12px;
    }
</style>