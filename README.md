[Uploading Index.html…]()```html
<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Eco Quatro | Water Treatment Solutions</title>

    <meta name="description"
        content="Eco Quatro menyediakan solusi pengelolaan dan jasa water treatment untuk kebutuhan industri, komersial, dan lingkungan.">

    <style>

        /* =====================================================
           RESET
        ===================================================== */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: #f5f7f2;
            color: #10140f;
            line-height: 1.5;
            overflow-x: hidden;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        img {
            max-width: 100%;
            display: block;
        }


        /* =====================================================
           VARIABLES
        ===================================================== */

        :root {
            --green: #163d2b;
            --green-light: #dce9df;
            --lime: #d9edc9;
            --cream: #f5f7f2;
            --dark: #10140f;
            --gray: #626962;
            --white: #ffffff;
            --border: #dfe4dd;
        }


        /* =====================================================
           NAVBAR
        ===================================================== */

        .navbar {
            position: fixed;
            top: 0;
            left: 0;

            width: 100%;

            padding: 22px 5%;

            display: flex;
            align-items: center;
            justify-content: space-between;

            z-index: 999;

            background: rgba(245, 247, 242, 0.88);
            backdrop-filter: blur(16px);

            border-bottom: 1px solid rgba(0, 0, 0, 0.05);
        }

        .logo {
            font-size: 24px;
            font-weight: 800;
            letter-spacing: -1.5px;
        }

        .logo span {
            color: #3f7652;
        }

        .nav-menu {
            display: flex;
            gap: 34px;
            align-items: center;
        }

        .nav-menu a {
            font-size: 14px;
            font-weight: 500;

            transition: 0.3s ease;
        }

        .nav-menu a:hover {
            opacity: 0.5;
        }

        .nav-right {
            display: flex;
            align-items: center;
            gap: 18px;
        }

        .nav-language {
            font-size: 13px;
            color: var(--gray);
        }

        .nav-button {
            background: var(--dark);
            color: white;

            padding: 12px 21px;

            border-radius: 50px;

            font-size: 13px;
            font-weight: 600;

            transition: 0.3s ease;
        }

        .nav-button:hover {
            transform: translateY(-2px);
            background: var(--green);
        }


        /* =====================================================
           HERO
        ===================================================== */

        .hero {
            min-height: 100vh;

            padding: 155px 5% 70px;

            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;

            text-align: center;
        }

        .eyebrow {
            text-transform: uppercase;

            font-size: 12px;
            letter-spacing: 3px;

            color: #69726b;

            margin-bottom: 25px;
        }

        .hero h1 {
            max-width: 1050px;

            font-size: clamp(58px, 8.5vw, 125px);

            line-height: 0.88;

            letter-spacing: -7px;

            font-weight: 700;

            margin-bottom: 35px;
        }

        .hero h1 span {
            color: #416f50;
        }

        .hero-description {
            max-width: 650px;

            font-size: 18px;

            color: var(--gray);

            margin-bottom: 35px;
        }

        .hero-buttons {
            display: flex;
            justify-content: center;

            gap: 12px;

            flex-wrap: wrap;
        }

        .button {
            padding: 15px 28px;

            border-radius: 50px;

            font-size: 14px;

            font-weight: 600;

            transition: 0.3s ease;
        }

        .button-dark {
            background: var(--dark);
            color: white;
        }

        .button-light {
            background: white;
            border: 1px solid var(--border);
        }

        .button:hover {
            transform: translateY(-3px);
        }


        /* =====================================================
           HERO IMAGE
        ===================================================== */

        .hero-image {
            width: 92%;
            max-width: 1300px;

            height: 600px;

            margin-top: 80px;

            border-radius: 32px;

            overflow: hidden;

            position: relative;

            background:
                linear-gradient(
                    rgba(15, 45, 29, 0.08),
                    rgba(15, 45, 29, 0.08)
                ),
                url("https://wastecinternational.com/wp-content/uploads/2025/01/5-1024x683.jpg");

            background-size: cover;
            background-position: center;
        }

        .hero-card {
            position: absolute;

            left: 30px;
            bottom: 30px;

            background: rgba(255,255,255,0.92);

            backdrop-filter: blur(12px);

            padding: 20px 25px;

            border-radius: 18px;

            text-align: left;
        }

        .hero-card strong {
            display: block;

            font-size: 24px;

            letter-spacing: -1px;
        }

        .hero-card span {
            font-size: 13px;

            color: #69726b;
        }


        /* =====================================================
           GENERAL SECTION
        ===================================================== */

        section {
            padding: 135px 5%;
        }

        .section-label {
            text-transform: uppercase;

            font-size: 12px;

            letter-spacing: 2.5px;

            color: #707970;

            margin-bottom: 25px;
        }

        .section-title {
            max-width: 1000px;

            font-size: clamp(45px, 6.5vw, 90px);

            line-height: 0.93;

            letter-spacing: -5px;

            margin-bottom: 60px;
        }


        /* =====================================================
           ABOUT
        ===================================================== */

        .about {
            background: var(--cream);
        }

        .about-content {
            max-width: 950px;

            font-size: 25px;

            line-height: 1.35;

            color: #3f4740;
        }

        .about-content strong {
            color: var(--green);
        }


        /* =====================================================
           SERVICES
        ===================================================== */

        .services {
            background: white;
        }

        .service-intro {
            max-width: 800px;

            font-size: 20px;

            color: var(--gray);

            margin-bottom: 70px;
        }

        .service-grid {
            display: grid;

            grid-template-columns: repeat(3, 1fr);

            gap: 18px;
        }

        .service-card {
            min-height: 510px;

            background: var(--cream);

            border-radius: 28px;

            padding: 35px;

            display: flex;
            flex-direction: column;
            justify-content: space-between;

            overflow: hidden;

            transition: 0.4s ease;
        }

        .service-card:hover {
            transform: translateY(-8px);
        }

        .service-number {
            font-size: 12px;

            color: #7a827b;

            letter-spacing: 1px;
        }

        .service-card h3 {
            font-size: 39px;

            letter-spacing: -2px;

            margin-bottom: 12px;
        }

        .service-card p {
            color: #687069;

            max-width: 330px;
        }

        .service-image {
            height: 210px;

            margin-top: 30px;

            border-radius: 20px;

            background-size: cover;

            background-position: center;
        }

        .water-treatment {
            background-image:
                url("https://upload.wikimedia.org/wikipedia/commons/4/4f/La_Crosse_wastewater_treatment_facility-2.jpg?utm_source=en.wikipedia.org&utm_campaign=index&utm_content=original");
        }

        .water-management {
            background-image:
                url("https://www.watercolormanagement.com/wp-content/uploads/2019/02/Water-Treatment-Industry-2019-Outlook-e1550174082146.jpg");
        }

        .maintenance {
            background-image:
                url("https://tigernix.com.au/wp-content/uploads/2023/12/importance-corrective-maintenance-water-treatment-infrastructure-tigernix-australia.jpg");
        }


        /* =====================================================
           SOLUTIONS / INDUSTRIES
        ===================================================== */

        .industries {
            background: var(--green);

            color: white;
        }

        .industries .section-label {
            color: #aabaae;
        }

        .industry-grid {
            display: grid;

            grid-template-columns: repeat(4, 1fr);

            gap: 15px;
        }

        .industry-card {
            min-height: 510px;

            border-radius: 26px;

            overflow: hidden;

            position: relative;

            display: flex;
            align-items: flex-end;

            padding: 28px;

            background-size: cover;
            background-position: center;

            transition: 0.4s ease;
        }

        .industry-card:hover {
            transform: translateY(-6px);
        }

        .industry-card::before {
            content: "";

            position: absolute;

            inset: 0;

            background:
                linear-gradient(
                    transparent 25%,
                    rgba(0,0,0,0.75)
                );
        }

        .industry-content {
            position: relative;

            z-index: 2;
        }

        .industry-content h3 {
            font-size: 30px;

            letter-spacing: -1px;

            margin-bottom: 5px;
        }

        .industry-content p {
            color: #d7ddd8;

            font-size: 13px;
        }

        .industrial {
            background-image:
                url("https://www.pwc.com/us/en/july-launch/gettyimages-1186335951_1600x900.png");
        }

        .commercial {
            background-image:
                url("https://magelangekspres.disway.id/upload/0a50168a705468bb74d96e54c440809e.jpeg");
        }

        .residential {
            background-image:
                url("https://propertyklik.com/tips-properti/wp-content/uploads/2024/05/komplek-perumahan-2-1024x576.jpeg");
        }

        .environment {
            background-image:
                url("https://akm-img-a-in.tosshub.com/indiatoday/images/story/202401/8-real-world-strategies-for-students-to-create-a-sustainable-planet-031719294-16x9_0.jpg?VersionId=CGeyfrs.3zRDUQTzqlO1GPe8CEOBNav2&size=690:388");
        }


        /* =====================================================
           SOLUTIONS
        ===================================================== */

        .solutions {
            background: #eef2eb;
        }

        .solution-grid {
            display: grid;

            grid-template-columns: 1fr 1fr;

            gap: 20px;
        }

        .solution-card {
            min-height: 620px;

            border-radius: 30px;

            position: relative;

            overflow: hidden;

            background-size: cover;
            background-position: center;
        }

        .solution-industry {
            background-image:
                url("https://d91ztqmtx7u1k.cloudfront.net/ClientContent/Images/ExtraLarge/industrial-water-treatment-pla-20241011113605110.jpg");
        }

        .solution-community {
            background-image:
                url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSZSC923sjkHxLv3Wd9jocungObEZJjamunGfF0qOa-skW_FHDVXWjtIDxc&s=10");
        }

        .solution-card::before {
            content: "";

            position: absolute;

            inset: 0;

            background:
                linear-gradient(
                    transparent 25%,
                    rgba(0,0,0,0.82)
                );
        }

        .solution-content {
            position: absolute;

            left: 40px;
            right: 40px;
            bottom: 40px;

            z-index: 2;

            color: white;
        }

        .solution-content h3 {
            font-size: 46px;

            letter-spacing: -2.5px;

            margin-bottom: 15px;
        }

        .solution-content p {
            max-width: 470px;

            color: #dedede;

            margin-bottom: 25px;
        }

        .solution-link {
            display: inline-block;

            padding: 13px 21px;

            border-radius: 50px;

            background: white;

            color: #111;

            font-size: 13px;

            font-weight: 600;
        }


        /* =====================================================
           WATER QUALITY DATA
        ===================================================== */

        .data-section {
            background: white;
        }

        .data-layout {
            display: grid;

            grid-template-columns: 1fr 1fr;

            gap: 90px;

            align-items: center;
        }

        .data-text h2 {
            font-size: clamp(45px, 6vw, 80px);

            line-height: 0.93;

            letter-spacing: -4px;

            margin-bottom: 30px;
        }

        .data-text p {
            max-width: 530px;

            font-size: 17px;

            color: var(--gray);
        }

        .water-dashboard {
            background: var(--cream);

            border-radius: 28px;

            padding: 35px;
        }

        .dashboard-title {
            font-size: 13px;

            color: #687069;

            margin-bottom: 30px;
        }

        .quality-row {
            margin-bottom: 28px;
        }

        .quality-label {
            display: flex;

            justify-content: space-between;

            font-size: 13px;

            margin-bottom: 9px;
        }

        .quality-bar {
            height: 18px;

            background: #dfe4de;

            border-radius: 20px;

            overflow: hidden;
        }

        .quality-fill {
            height: 100%;

            border-radius: 20px;

            background: var(--green);
        }

        .tss {
            width: 72%;
        }

        .cod {
            width: 58%;
        }

        .bod {
            width: 42%;
        }


        /* =====================================================
           PROCESS
        ===================================================== */

        .process {
            background: #e0eadf;
        }

        .process-grid {
            display: grid;

            grid-template-columns: repeat(3, 1fr);

            gap: 18px;
        }
        

        .process-card {
            background: white;

            border-radius: 26px;

            min-height: 390px;

            padding: 32px;

            display: flex;
            flex-direction: column;
        
        } 

        .process-number {
            width: 42px;
            height: 42px;

            display: flex;

            justify-content: center;
            align-items: center;

            border-radius: 50%;

            background: var(--green);

            color: white;

            font-size: 13px;
        }

        .process-card h3 {
            font-size: 31px;

            letter-spacing: -1px;

            margin-bottom: 12px;
        }

        .process-card p {
            color: #687069;
        }




        /* =====================================================
           ABOUT COMPANY
        ===================================================== */

        .company {
            background: #10140f;

            color: white;

            text-align: center;
        }

        .company .section-label {
            color: #8d998f;
        }

        .company h2 {
            max-width: 1000px;

            margin: auto;

            font-size: clamp(50px, 7vw, 105px);

            line-height: 0.9;

            letter-spacing: -6px;
        }

        .company h2 span {
            color: #a9d3ad;
        }

        .company-description {
            max-width: 650px;

            margin: 40px auto 0;

            color: #aeb5af;

            font-size: 18px;
        }


        /* =====================================================
           CTA
        ===================================================== */

        .cta {
            min-height: 680px;

            display: flex;

            justify-content: center;

            align-items: center;

            text-align: center;

            background:
                radial-gradient(
                    circle at center,
                    #cfe5cf,
                    #f5f7f2 62%
                );
        }

        .cta-content {
            max-width: 950px;
        }

        .cta h2 {
            font-size: clamp(55px, 8vw, 110px);

            line-height: 0.9;

            letter-spacing: -6px;

            margin-bottom: 35px;
        }

        .cta p {
            max-width: 600px;

            margin: auto auto 35px;

            color: var(--gray);

            font-size: 18px;
        }


        /* =====================================================
           FOOTER
        ===================================================== */

        footer {
            background: #10140f;

            color: white;

            padding: 75px 5% 30px;
        }

        .footer-grid {
            display: grid;

            grid-template-columns: 2fr 1fr 1fr 1fr;

            gap: 50px;

            margin-bottom: 80px;
        }

        .footer-logo {
            font-size: 31px;

            font-weight: 800;

            letter-spacing: -2px;
        }

        .footer-description {
            max-width: 310px;

            color: #858e87;

            margin-top: 20px;
        }

        .footer-column h4 {
            font-size: 11px;

            text-transform: uppercase;

            letter-spacing: 2px;

            color: #687169;

            margin-bottom: 20px;
        }

        .footer-column a {
            display: block;

            font-size: 14px;

            color: #d7ddd8;

            margin-bottom: 12px;

            transition: 0.3s;
        }

        .footer-column a:hover {
            color: white;

            transform: translateX(3px);
        }

        .footer-bottom {
            border-top: 1px solid #2c322d;

            padding-top: 25px;

            display: flex;

            justify-content: space-between;

            color: #697169;

            font-size: 12px;
        }




        /* =====================================================
           RESPONSIVE TABLET
        ===================================================== */

        @media (max-width: 950px) {

            .nav-menu {
                display: none;
            }

            .service-grid {
                grid-template-columns: 1fr;
            }

            .industry-grid {
                grid-template-columns: 1fr 1fr;
            }

            .solution-grid {
                grid-template-columns: 1fr;
            }

            .data-layout {
                grid-template-columns: 1fr;

                gap: 50px;
            }

            .process-grid {
                grid-template-columns: 1fr;
            }

            .footer-grid {
                grid-template-columns: 1fr 1fr;
            }
        }





        /* =====================================================
           RESPONSIVE MOBILE
        ===================================================== */

        @media (max-width: 600px) {

            .navbar {
                padding: 18px 5%;
            }

            .nav-language {
                display: none;
            }

            .hero {
                padding-top: 130px;
            }

            .hero h1 {
                font-size: 52px;

                letter-spacing: -3.5px;
            }

            .hero-description {
                font-size: 16px;
            }

            .hero-image {
                width: 100%;

                height: 430px;

                margin-top: 50px;

                border-radius: 24px;
            }

            section {
                padding: 90px 5%;
            }

            .section-title {
                font-size: 52px;

                letter-spacing: -3px;
            }

            .about-content {
                font-size: 20px;
            }

            .industry-grid {
                grid-template-columns: 1fr;
            }

            .industry-card {
                min-height: 400px;
            }

            .solution-card {
                min-height: 470px;
            }

            .solution-content {
                left: 25px;
                right: 25px;
                bottom: 25px;
            }

            .solution-content h3 {
                font-size: 36px;
            }

            .cta {
                min-height: 550px;
            }

            .cta h2 {
                font-size: 58px;

                letter-spacing: -3px;
            }

            .footer-grid {
                grid-template-columns: 1fr;
            }

            .footer-bottom {
                flex-direction: column;

                gap: 10px;
            }
        }

    </style>

</head>


<body>


    <!-- =====================================================
         NAVIGATION
    ===================================================== -->

    <nav class="navbar">

        <a href="#" class="logo">
            ECO <span>QUATRO</span>
        </a>

        <div class="nav-menu">

            <a href="#services">
                Services
            </a>

            <a href="#solutions">
                Solutions
            </a>

            <a href="#industries">
                Industries
            </a>

            <a href="#about">
                About
            </a>

        </div>


        <div class="nav-right">

            <span class="nav-language">
                ID
            </span>

            <a href="#contact" class="nav-button">
                Konsultasi
            </a>

        </div>

    </nav>


    <!-- =====================================================
         HERO
    ===================================================== -->

    <main>

        <section class="hero">

            <div class="eyebrow">
                Water Treatment Solutions · Est. 2026
            </div>

            <h1>
                The Water
                Solution for a
                <span>Better Future.</span>
            </h1>

            <p class="hero-description">
                Eco Quatro menghadirkan solusi pengelolaan dan
                jasa water treatment yang membantu industri,
                bisnis, dan lingkungan mendapatkan kualitas air
                yang lebih baik dan berkelanjutan.
            </p>

            <div class="hero-buttons">

                <a href="#services" class="button button-dark">
                    Lihat Layanan
                </a>

                <a href="#contact" class="button button-light">
                    Konsultasi Proyek
                </a>

            </div>


            <div class="hero-image">

                <div class="hero-card">

                    <strong>
                        Water. Managed Better.
                    </strong>

                    <span>
                        Integrated Water Treatment Solutions
                    </span>

                </div>

            </div>

        </section>


        <!-- =================================================
             ABOUT INTRO
        ================================================= -->

        <section class="about" id="about">

            <div class="section-label">
                About Eco Quatro
            </div>

            <h2 class="section-title">
                Mengelola air dengan
                pendekatan yang lebih
                cerdas.
            </h2>

            <div class="about-content">

                <p>
                    <strong>Eco Quatro</strong> adalah perusahaan
                    yang didirikan pada tahun <strong>2026</strong>
                    dengan fokus pada pengelolaan, pengolahan,
                    dan jasa water treatment.
                </p>

                <br>

                <p>
                    Kami menggabungkan pendekatan engineering,
                    teknologi pengolahan air, monitoring, dan
                    maintenance untuk menciptakan sistem
                    pengelolaan air yang efektif, efisien,
                    dan berkelanjutan.
                </p>

            </div>

        </section>


        <!-- =================================================
             SERVICES
        ================================================= -->

        <section class="services" id="services">

            <div class="section-label">
                What We Do
            </div>

            <h2 class="section-title">
                One partner for
                your water needs.
            </h2>

            <p class="service-intro">
                Dari perencanaan sistem hingga pengoperasian
                dan pemeliharaan, Eco Quatro menyediakan
                layanan water treatment yang dapat disesuaikan
                dengan kebutuhan setiap proyek.
            </p>


            <div class="service-grid">


                <!-- CARD 01 -->

                <div class="service-card">

                    <div class="service-number">
                        01 / WATER TREATMENT
                    </div>

                    <div>

                        <h3>
                            Water Treatment
                        </h3>

                        <p>
                            Perencanaan dan pengelolaan sistem
                            pengolahan air untuk menghasilkan
                            kualitas air sesuai kebutuhan.
                        </p>

                        <div class="service-image water-treatment">
                        </div>

                    </div>

                </div>


                <!-- CARD 02 -->

                <div class="service-card">

                    <div class="service-number">
                        02 / WATER MANAGEMENT
                    </div>

                    <div>

                        <h3>
                            Water Management
                        </h3>

                        <p>
                            Pengelolaan penggunaan air secara
                            efektif melalui monitoring,
                            evaluasi, dan optimasi sistem.
                        </p>

                        <div class="service-image water-management">
                        </div>

                    </div>

                </div>


                <!-- CARD 03 -->

                <div class="service-card">

                    <div class="service-number">
                        03 / MAINTENANCE
                    </div>

                    <div>

                        <h3>
                            Maintenance
                        </h3>

                        <p>
                            Pemeriksaan, perawatan, dan
                            optimalisasi sistem agar fasilitas
                            water treatment tetap bekerja
                            secara konsisten.
                        </p>

                        <div class="service-image maintenance">
                        </div>

                    </div>

                </div>

            </div>

        </section>


        <!-- =================================================
             INDUSTRIES
        ================================================= -->

        <section class="industries" id="industries">

            <div class="section-label">
                Where We Work
            </div>

            <h2 class="section-title">
                Water solutions
                for every environment.
            </h2>


            <div class="industry-grid">


                <div class="industry-card industrial">

                    <div class="industry-content">

                        <h3>
                            Industrial
                        </h3>

                        <p>
                            Water treatment untuk kebutuhan
                            proses industri.
                        </p>

                    </div>

                </div>


                <div class="industry-card commercial">

                    <div class="industry-content">

                        <h3>
                            Commercial
                        </h3>

                        <p>
                            Solusi pengelolaan air untuk
                            gedung dan fasilitas bisnis.
                        </p>

                    </div>

                </div>


                <div class="industry-card residential">

                    <div class="industry-content">

                        <h3>
                            Residential
                        </h3>

                        <p>
                            Sistem pengolahan air untuk
                            kebutuhan hunian.
                        </p>

                    </div>

                </div>


                <div class="industry-card environment">

                    <div class="industry-content">

                        <h3>
                            Environment
                        </h3>

                        <p>
                            Solusi pengelolaan air yang
                            memperhatikan keberlanjutan.
                        </p>

                    </div>

                </div>

            </div>

        </section>


        <!-- =================================================
             SOLUTIONS
        ================================================= -->

        <section class="solutions" id="solutions">

            <div class="section-label">
                Our Solutions
            </div>

            <h2 class="section-title">
                Designed around
                your water system.
            </h2>


            <div class="solution-grid">


                <!-- INDUSTRIAL -->

                <div class="solution-card solution-industry">

                    <div class="solution-content">

                        <h3>
                            Industrial Solutions
                        </h3>

                        <p>
                            Sistem water treatment yang dirancang
                            berdasarkan karakteristik air,
                            kapasitas, proses produksi, dan
                            kebutuhan operasional industri.
                        </p>

                        <a href="#contact"
                           class="solution-link">

                            Explore Solution →

                        </a>

                    </div>

                </div>


                <!-- COMMUNITY -->

                <div class="solution-card solution-community">

                    <div class="solution-content">

                        <h3>
                            Sustainable Water
                        </h3>

                        <p>
                            Membantu fasilitas dan lingkungan
                            mengelola sumber daya air secara
                            lebih efisien dan bertanggung jawab.
                        </p>

                        <a href="#contact"
                           class="solution-link">

                            Explore Solution →

                        </a>

                    </div>

                </div>

            </div>

        </section>


        <!-- =================================================
             WATER QUALITY
        ================================================= -->

        <section class="data-section">

            <div class="data-layout">


                <div class="data-text">

                    <div class="section-label">
                        Water Quality
                    </div>

                    <h2>
                        Better water
                        starts with
                        better data.
                    </h2>

                    <p>
                        Monitoring parameter kualitas air membantu
                        memahami kondisi sistem secara lebih
                        menyeluruh. Data dapat menjadi dasar untuk
                        menentukan tindakan pengolahan,
                        maintenance, dan optimasi berikutnya.
                    </p>

                </div>


                <div class="water-dashboard">

                    <div class="dashboard-title">
                        Example Water Quality Monitoring
                    </div>

                    <div class="quality-row">

                        <div class="quality-label">

                            <span>
                                TSS Control
                            </span>

                            <span>
                                72%
                            </span>

                        </div>

                        <div class="quality-bar">

                            <div class="quality-fill tss">
                            </div>

                        </div>

                    </div>


                    <div class="quality-row">

                        <div class="quality-label">

                            <span>
                                COD Reduction
                            </span>

                            <span>
                                58%
                            </span>

                        </div>

                        <div class="quality-bar">

                            <div class="quality-fill cod">
                            </div>

                        </div>

                    </div>


                    <div class="quality-row">

                        <div class="quality-label">

                            <span>
                                BOD Reduction
                            </span>

                            <span>
                                42%
                            </span>

                        </div>

                        <div class="quality-bar">

                            <div class="quality-fill bod">
                            </div>

                        </div>

                    </div>

                </div>

            </div>

        </section>


        <!-- =================================================
             PROCESS
        ================================================= -->

        <section class="process">

            <div class="section-label">
                How We Work
            </div>

            <h2 class="section-title">
                From water problem
                to practical solution.
            </h2>


            <div class="process-grid">


                <div class="process-card">

                    <div class="process-number">
                        01
                    </div>

                    <div>

                        <h3>
                            Assessment
                        </h3>

                        <p>
                            Kami mempelajari karakteristik air,
                            kebutuhan pengguna, kapasitas sistem,
                            dan permasalahan yang terjadi.
                        </p>

                    </div>

                </div>


                <div class="process-card">

                    <div class="process-number">
                        02
                    </div>

                    <div>

                        <h3>
                            Engineering
                        </h3>

                        <p>
                            Data yang diperoleh digunakan untuk
                            merancang pendekatan pengolahan air
                            yang sesuai dengan kebutuhan proyek.
                        </p>

                    </div>

                </div>


                <div class="process-card">

                    <div class="process-number">
                        03
                    </div>

                    <div>

                        <h3>
                            Operation
                        </h3>

                        <p>
                            Sistem kemudian dapat dioperasikan,
                            dimonitor, dirawat, dan dievaluasi
                            secara berkala.
                        </p>

                    </div>

                </div>

            </div>

        </section>


        <!-- =================================================
             COMPANY
        ================================================= -->

        <section class="company">

            <div class="section-label">
                Eco Quatro · Since 2026
            </div>

            <h2>
                Engineering water
                for a <span>greener future.</span>
            </h2>

            <p class="company-description">

                Sebagai perusahaan yang berdiri pada tahun 2026,
                Eco Quatro hadir dengan semangat untuk menghadirkan
                solusi water treatment yang menggabungkan teknologi,
                engineering, efisiensi, dan kepedulian terhadap
                lingkungan.

            </p>

        </section>


        <!-- =================================================
             CTA
        ================================================= -->

        <section class="cta" id="contact">

            <div class="cta-content">

                <div class="section-label">
                    Start Your Project
                </div>

                <h2>
                    Let's build a
                    better water system.
                </h2>

                <p>
                    Diskusikan kebutuhan water treatment,
                    pengelolaan air, atau maintenance sistem
                    bersama tim Eco Quatro.
                </p>

                <a href="https://wa.link/cl5lwl"
                   class="button button-dark">

                    Konsultasi dengan Eco Quatro →

                </a>

            </div>

        </section>

    </main>


    <!-- =====================================================
         FOOTER
    ===================================================== -->

    <footer>

        <div class="footer-grid">


            <div>

                <div class="footer-logo">
                    ECO QUATRO
                </div>

                <p class="footer-description">

                    Water treatment and management solutions
                    for a cleaner, more efficient, and
                    sustainable future.

                </p>

            </div>


            <div class="footer-column">

                <h4>
                    Services
                </h4>

                <a href="#services">
                    Water Treatment
                </a>

                <a href="#services">
                    Water Management
                </a>

                <a href="#services">
                    Maintenance
                </a>

            </div>


            <div class="footer-column">

                <h4>
                    Company
                </h4>

                <a href="#about">
                    About Eco Quatro
                </a>

                <a href="#solutions">
                    Solutions
                </a>

                <a href="#industries">
                    Industries
                </a>

            </div>


            <div class="footer-column">

                <h4>
                    Contact
                </h4>

                <a href="mailto:ecoquatro.idn@gmail.com">
                    Email
                </a>

                <a href="https://www.instagram.com/ecoquatro.idn?stkn=c2o2dm45N3VhdHo=">
                    Instagram
                </a>

            </div>

        </div>


        <div class="footer-bottom">

            <span>
                © 2026 Eco Quatro All rights reserved.
            </span>

            <span>
                Water · Engineering · Sustainability
            </span>

        </div>

    </footer>


</body>

</html>
```

