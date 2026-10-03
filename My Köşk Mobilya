<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Köşk Mobilya | Mustafa Yürük</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
            scroll-behavior: smooth;
        }
        body {
            background-color: #f7f4ed;
            color: #2c221e;
            line-height: 1.6;
        }

        /* Sabit Üst Menü */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: rgba(15, 10, 6, 0.95);
            backdrop-filter: blur(10px);
            color: #fff;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 12px 20px;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.3);
            border-bottom: 1px solid rgba(212, 175, 55, 0.3);
        }
        .brand-title {
            font-size: 15px;
            font-weight: 700;
            color: #d4af37;
            cursor: pointer;
        }
        .header-menu {
            display: flex;
            gap: 10px;
        }
        .header-menu button {
            background: #d4af37;
            color: #1e140c;
            padding: 6px 12px;
            border: none;
            border-radius: 20px;
            font-size: 12px;
            font-weight: 600;
            cursor: pointer;
            transition: 0.3s;
        }
        .header-menu button:hover {
            background: #e6c55c;
        }

        /* Sayfa Yönetimi */
        .page {
            display: none;
            max-width: 600px;
            margin: 85px auto 40px auto;
            padding: 20px;
        }
        .page.active {
            display: block;
        }

        /* Hero / Başlık Alanı */
        .hero-section {
            background: linear-gradient(rgba(15, 10, 6, 0.85), rgba(15, 10, 6, 0.85)), url('https://images.unsplash.com/photo-1618221195710-dd6b41faaea6?auto=format&fit=crop&w=800&q=80');
            background-size: cover;
            background-position: center;
            border-radius: 16px;
            padding: 30px 20px;
            margin-bottom: 20px;
            text-align: center;
            color: #fff;
            border: 1px solid rgba(212, 175, 55, 0.4);
            box-shadow: 0 8px 25px rgba(0,0,0,0.3);
        }
        .hero-section h1 {
            font-size: 18px;
            color: #d4af37;
            margin-bottom: 8px;
            line-height: 1.4;
        }
        .hero-section p {
            font-size: 14px;
            color: #d1c7bd;
            font-weight: 600;
        }

        /* Bölüm Kutuları */
        .section {
            background: #ffffff;
            border-radius: 16px;
            padding: 25px 20px;
            margin-bottom: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            border: 1px solid #e8e1d5;
        }
        .section h2 {
            color: #4a3319;
            font-size: 18px;
            margin-bottom: 12px;
            border-bottom: 2px solid #d4af37;
            display: inline-block;
            padding-bottom: 4px;
        }
        .section p {
            font-size: 14px;
            color: #444;
            margin-bottom: 12px;
            line-height: 1.6;
        }

        /* İçerik İçi Mobilya Görselleri */
        .content-img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            border-radius: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
        }

        /* Hizmet Kutuları */
        .features-grid {
            display: flex;
            gap: 10px;
            margin-top: 15px;
        }
        .feature-box {
            flex: 1;
            background: #fdfbf7;
            padding: 12px;
            border-radius: 10px;
            border: 1px solid #e8e1d5;
            text-align: center;
        }
        .feature-box h3 {
            font-size: 14px;
            color: #4a3319;
            margin-bottom: 6px;
        }
        .feature-box p {
            font-size: 11px;
            color: #666;
            margin: 0;
        }

        /* Ülkeler Listesi Tasarımı */
        .countries-box {
            background: #faf7f0;
            border: 1px solid #e8e1d5;
            border-radius: 10px;
            padding: 15px;
            max-height: 220px;
            overflow-y: auto;
            font-size: 13px;
            color: #555;
            line-height: 1.8;
        }

        /* Sosyal Medya & Butonlar */
        .social-links {
            display: flex;
            flex-direction: column;
            gap: 10px;
            margin-top: 15px;
        }
        .social-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            background: #2c221e;
            color: #fff;
            text-decoration: none;
            padding: 12px;
            border-radius: 10px;
            font-size: 14px;
            font-weight: 600;
            transition: 0.3s;
        }
        .social-btn:hover {
            background: #d4af37;
            color: #1e140c;
        }

        /* Tıklanamaz Bilgi Kutusu (Gmail İçin) */
        .info-box {
            background: #faf7f0;
            border: 1px solid #d4af37;
            color: #4a3319;
            padding: 14px;
            border-radius: 10px;
            font-size: 14px;
            font-weight: 600;
            text-align: center;
        }

        .footer {
            text-align: center;
            font-size: 12px;
            color: #888;
            margin-top: 30px;
        }
    </style>
</head>
<body>

    <!-- Sabit Üst Menü -->
    <header>
        <div class="brand-title" onclick="switchPage('home')">My Köşk Mobilya</div>
        <div class="header-menu">
            <button onclick="switchPage('contact')">İletişim</button>
        </div>
    </header>

    <!-- 1. SAYFA: ANA SAYFA -->
    <div id="home-page" class="page active">
        
        <!-- Üst Bilgi Alanı (Profil Fotoğrafsız, Yazılı) -->
        <div class="hero-section">
            <h1>My Köşk Mobilya İnşaat Sanayi Ticaret Ltd.</h1>
            <p>Mustafa Yürük</p>
        </div>

        <div class="section">
            <h2>Hoş Geldiniz, Ben Mustafa Yürük</h2>
            <p>Değerli misafirlerimiz, ben ve profesyonel ekibimle birlikte uzun yıllardır mobilya sektöründe zirveyi hedefliyoruz. My Köşk Mobilya olarak evlerinize sadece eşya değil, zarafet, konfor ve prestij katıyoruz.</p>
            <img src="https://images.unsplash.com/photo-1555041469-a586c61ea9bc?auto=format&fit=crop&w=800&q=80" alt="Lüks Mobilya" class="content-img">
            <p>Kendi imalathanemizde, usta ellerin ve en kaliteli malzemelerin buluştuğu tasarımlarımızı hayata geçiriyoruz. Standart kalıpların dışına çıkarak hayalinizdeki yaşam alanını birebir üretiyoruz.</p>
        </div>

        <div class="section">
            <h2>Showroom & Özel Ölçü İmalat</h2>
            <p>Tarzınıza en uygun modelleri inceleyebileceğiniz özel <strong>showroom mağazamız</strong> ve üretim gücümüzü sergilediğimiz <strong>imalathanemiz</strong> ile hizmetinizdeyiz.</p>
            
            <div class="features-grid">
                <div class="feature-box">
                    <h3>Showroom Mağaza</h3>
                    <p>Ürünlerimizi yerinde görün, kalitemizi yakından hissedin.</p>
                </div>
                <div class="feature-box">
                    <h3>Özel Ölçü Tasarım</h3>
                    <p>Evinizin ölçülerine ve zevkinize özel imalat yapıyoruz.</p>
                </div>
            </div>
            <img src="https://images.unsplash.com/photo-1524758631624-e2822e304c36?auto=format&fit=crop&w=800&q=80" alt="Mobilya İmalat" class="content-img">
        </div>

        <div class="section">
            <h2>🌍 Küresel Hizmet Ağımız</h2>
            <p>Sadece Türkiye'de değil, dünyanın dört bir yanında global standartlarda hizmet veriyoruz. Aktif olarak hizmet sağladığımız ülkeler:</p>
            
            <div class="countries-box">
                🇹🇷 Türkiye, 🇦🇫 Afganistan, 🇩🇪 Almanya, 🇺🇸 Amerika Birleşik Devletleri, 🇦🇩 Andorra, 🇦🇴 Angola, 🇦🇬 Antigua ve Barbuda, 🇦🇷 Arjantin, 🇦🇱 Arnavutluk, 🇦🇺 Avustralya, 🇦🇹 Avusturya, 🇦🇿 Azerbaycan, 🇧🇸 Bahamalar, 🇧🇭 Bahreyn, 🇧🇩 Bangladeş, 🇧🇧 Barbados, 🇧🇾 Belarus, 🇧🇪 Belçika, 🇧🇿 Belize, 🇧🇯 Benin, 🇧🇹 Bhutan, 🇦🇪 Birleşik Arap Emirlikleri, 🇬🇧 Birleşik Krallık, 🇧🇴 Bolivya, 🇧🇦 Bosna-Hersek, 🇧🇼 Botsvana, 🇧🇷 Brezilya, 🇧🇳 Brunei, 🇧🇬 Bulgaristan, 🇧🇫 Burkina Faso, 🇧🇮 Burundi, 🇨🇻 Cabo Verde, 🇩🇯 Cibuti, 🇹🇩 Çad, 🇨🇿 Çekya, 🇨🇳 Çin, 🇩🇰 Danimarka, 🇩🇴 Dominik Cumhuriyeti, 🇩🇲 Dominika, 🇪🇨 Ekvador, 🇬🇶 Ekvator Ginesi, 🇸🇻 El Salvador, 🇮🇩 Endonezya, 🇪🇷 Eritre, 🇦🇲 Ermenistan, 🇪🇪 Estonya, 🇸🇿 Esvatini, 🇪🇹 Etiyopya, 🇫🇯 Fiji, 🇵🇭 Filipinler, 🇫🇮 Finlandiya, 🇫🇷 Fransa, 🇬🇦 Gabon, 🇬🇲 Gambiya, 🇬🇭 Gana, 🇬🇳 Gine, 🇬🇼 Gine-Bissau, 🇬🇩 Grenada, 🇬🇾 Guyana, 🇿🇦 Güney Afrika, 🇰🇷 Güney Kore, 🇸🇸 Güney Sudan, 🇬🇪 Gürcistan, 🇭🇹 Haiti, 🇭🇷 Hırvatistan, 🇮🇳 Hindistan, 🇳🇱 Hollanda, 🇭🇳 Honduras, 🇭🇺 Macaristan, 🇮🇶 Irak, 🇮🇷 İran, 🇮🇪 İrlanda, 🇪🇸 İspanya, 🇸🇪 İsveç, 🇨🇭 İsviçre, 🇮🇹 İtalya, 🇮🇸 İzlanda, 🇯🇲 Jamaika, 🇯🇵 Japonya, 🇰🇭 Kamboçya, 🇨🇲 Kamerun, 🇨🇦 Kanada, 🇲🇪 Karadağ, 🇶🇦 Katar, 🇰🇿 Kazakistan, 🇰🇪 Kenya, 🇨🇾 Kıbrıs, 🇰🇬 Kırgızistan, 🇨🇴 Kolombiya, 🇰🇲 Komorlar, 🇨🇬 Kongo Cumhuriyeti, 🇨🇩 Kongo Demokratik Cumhuriyeti, 🇨🇷 Kosta Rika, 🇰🇼 Kuveyt, 🇰🇺 Küba, 🇱🇦 Laos, 🇱🇸 Lesotho, 🇱🇻 Letonya, 🇱🇷 Liberya, 🇱🇾 Libya, 🇱🇮 Lihtenştayn, 🇱🇹 Litvanya, 🇱🇺 Lüksemburg, 🇲🇬 Madagaskar, 🇲🇼 Malavi, 🇲🇾 Malezya, 🇲🇻 Maldivler, 🇲🇱 Mali, 🇲🇹 Malta, 🇲🇭 Marshall Adaları, 🇲🇷 Moritanya, 🇲🇺 Mauritius, 🇲🇽 Meksika, 🇫🇲 Mikronezya, 🇲🇩 Moldova, 🇲🇨 Monako, 🇲🇳 Moğolistan, 🇲🇦 Fas, 🇲🇿 Mozambik, 🇲🇲 Myanmar, 🇳🇦 Namibya, 🇳🇷 Nauru, 🇳🇵 Nepal, 🇳🇪 Nijer, 🇳🇬 Nijerya, 🇳🇮 Nikaragua, 🇳🇴 Norveç, 🇨🇫 Orta Afrika Cumhuriyeti, 🇺🇿 Özbekistan, 🇵🇰 Pakistan, 🇵🇼 Palau, 🇵🇦 Panama, 🇵🇬 Papua Yeni Gine, 🇵🇾 Paraguay, 🇵🇪 Peru, 🇵🇱 Polonya, 🇵🇹 Portekiz, 🇷🇴 Romanya, 🇷🇺 Rusya, 🇷🇼 Ruanda, 🇰🇳 Saint Kitts ve Nevis, 🇱🇨 Saint Lucia, 🇻🇨 Saint Vincent ve Grenadinler, 🇼🇸 Samoa, 🇸🇲 San Marino, 🇸🇹 Sao Tome ve Principe, 🇸🇳 Senegal, 🇸🇨 Seyşeller, 🇷🇸 Sırbistan, 🇸🇱 Sierra Leone, 🇸🇬 Singapur, 🇸🇰 Slovakya, 🇸🇮 Slovenya, 🇸🇧 Solomon Adaları, 🇸🇴 Somali, 🇱🇰 Sri Lanka, 🇸🇩 Sudan, 🇸🇷 Surinam, 🇸🇾 Suriye, 🇸🇦 Suudi Arabistan, 🇹🇯 Tacikistan, 🇹🇿 Tanzanya, 🇹🇭 Tayland, 🇹🇱 Doğu Timor, 🇹🇬 Togo, 🇹🇴 Tonga, 🇹🇹 Trinidad ve Tobago, 🇹🇳 Tunus, 🇹🇲 Türkmenistan, 🇹🇻 Tuvalu, 🇺🇬 Uganda, 🇺🇦 Ukrayna, 🇴🇲 Umman, 🇺🇾 Uruguay, 🇯🇴 Ürdün, 🇻🇺 Vanuatu, 🇻🇦 Vatikan, 🇻🇪 Venezuela, 🇻🇳 Vietnam, 🇾🇪 Yemen, 🇳🇿 Yeni Zelanda, 🇿🇲 Zambiya, 🇿🇼 Zimbabve, 🇲🇰 Kuzey Makedonya, 🇵🇸 Filistin, 🇰🇵 Kuzey Kore, 🇱🇧 Lübnan.
            </div>
        </div>

        <!-- Ana Sayfa Sosyal Medya Alanı -->
        <div class="section">
            <h2>Sosyal Medya Kanallarımız</h2>
            <p>Projelerimizi ve videolarımızı yakından takip edin:</p>
            <div class="social-links">
                <a href="https://www.tiktok.com/@my.kosk.mobilya" target="_blank" class="social-btn">TikTok: @my.kosk.mobilya</a>
                <a href="https://www.youtube.com/@my_kosk_mobilya" target="_blank" class="social-btn">YouTube: @my_kosk_mobilya</a>
                <a href="https://www.instagram.com/my_kosk_mobilya?stkn=MWs5aDExbG51NmVjcQ%3D%3D&utm_source=qr" target="_blank" class="social-btn">Instagram: @my_kosk_mobilya</a>
                <a href="https://x.com/my_kosk_mobilya?s=11" target="_blank" class="social-btn">X (Twitter): @my_kosk_mobilya</a>
                <a href="https://pin.it/1S1m97Vrt" target="_blank" class="social-btn">Pinterest: My Köşk Mobilya</a>
            </div>
        </div>

        <div class="footer">
            &copy; 2026 My Köşk Mobilya İnşaat Sanayi Ticaret Ltd. - Tüm Hakları Saklıdır.
        </div>
    </div>


    <!-- 2. SAYFA: İLETİŞİM SAYFASI -->
    <div id="contact-page" class="page">
        <div class="section">
            <h2>İletişim Bilgileri</h2>
            <p>Bizimle e-posta yoluyla iletişim kurabilirsiniz.</p>
            
            <div class="social-links">
                <!-- Tıklanamaz Gmail Alanı (Düz Metin) -->
                <div class="info-box">
                    Gmail: mykoskmobilya1@gmail.com
                </div>
            </div>

            <div style="text-align: center; margin-top: 25px;">
                <button onclick="switchPage('home')" style="background: none; border: none; color: #4a3319; font-weight: bold; cursor: pointer; text-decoration: underline; font-size: 14px;">
                    &larr; Ana Sayfaya Geri Dön
                </button>
            </div>
        </div>

        <div class="footer">
            &copy; 2026 My Köşk Mobilya İnşaat Sanayi Ticaret Ltd. - Tüm Hakları Saklıdır.
        </div>
    </div>

    <!-- Sayfalar Arası Geçiş Scripti -->
    <script>
        function switchPage(pageName) {
            const homePage = document.getElementById('home-page');
            const contactPage = document.getElementById('contact-page');

            if (pageName === 'home') {
                homePage.classList.add('active');
                contactPage.classList.remove('active');
            } else if (pageName === 'contact') {
                contactPage.classList.add('active');
                homePage.classList.remove('active');
            }
            window.scrollTo(0, 0);
        }
    </script>

</body>
</html>
