<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
    <title>My Köşk Mobilya | Özel Ölçü Lüks Mobilya</title>
    <script defer src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/js/all.min.js"></script>
    <style>
        :root {
            --bg: #0a0a0a;
            --card: #141414;
            --line: #2a2418;
            --gold: #c9a24a;
            --gold2: #e6c878;
            --tx: #ece7dc;
            --mut: #9d9788;
        }
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        html {
            scroll-behavior: smooth;
            scroll-padding-top: 90px;
            height: 100%;
        }
        body {
            background: var(--bg);
            color: var(--tx);
            font-family: Georgia, 'Times New Roman', serif;
            line-height: 1.65;
            padding-top: env(safe-area-inset-top, 0px);
            padding-bottom: env(safe-area-inset-bottom, 0px);
        }
        .w {
            max-width: 1040px;
            margin: 0 auto;
            padding: 0 18px;
        }
        nav {
            position: sticky;
            top: env(safe-area-inset-top, 0px);
            z-index: 9;
            background: rgba(10, 10, 10, .92);
            backdrop-filter: blur(8px);
            border-bottom: 1px solid var(--line);
        }
        nav .w {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            gap: 4px 10px;
            padding-top: 9px;
            padding-bottom: 6px;
            min-height: 54px;
        }
        .lk {
            width: 100%;
            text-align: center;
            order: 3;
        }
        .lang {
            display: flex;
            border: 1px solid var(--gold);
            border-radius: 20px;
            overflow: hidden;
            font: 600 12px system-ui, sans-serif;
        }
        .lang button {
            background: none;
            border: 0;
            color: var(--tx);
            padding: 6px 10px;
            cursor: pointer;
            font: inherit;
        }
        .lang button.on {
            background: linear-gradient(135deg, var(--gold), var(--gold2));
            color: #111;
        }
        nav b {
            color: var(--gold);
            letter-spacing: .1em;
            font-size: 15px;
        }
        nav div a {
            color: var(--tx);
            text-decoration: none;
            font-size: 13px;
            margin: 0 8px;
            font-family: system-ui, sans-serif;
        }
        .hero {
            background: #000;
            text-align: center;
            padding: 36px 18px 48px;
            border-bottom: 1px solid var(--line);
        }
        .hero img {
            width: min(260px, 70%);
            height: auto;
        }
        .hero h1 {
            font-size: clamp(24px, 6vw, 40px);
            font-weight: 400;
            color: var(--gold2);
            letter-spacing: .06em;
            margin: 6px 0 10px;
        }
        .hero p {
            color: var(--mut);
            max-width: 560px;
            margin: 0 auto 22px;
            font-size: 16px;
        }
        .ww {
            display: inline-block;
            border: 1px solid var(--gold);
            color: var(--gold2);
            border-radius: 20px;
            padding: 6px 16px;
            margin: 0 0 18px;
            font: 13px system-ui, sans-serif;
        }
        .ww i, .ww svg {
            margin-right: 6px;
        }
        .btn {
            display: inline-block;
            background: linear-gradient(135deg, var(--gold), var(--gold2));
            color: #111;
            padding: 12px 26px;
            border-radius: 2px;
            text-decoration: none;
            font: 600 14px system-ui, sans-serif;
            letter-spacing: .06em;
            border: 0;
            cursor: pointer;
        }
        .btn.o {
            background: none;
            color: var(--gold);
            border: 1px solid var(--gold);
            margin-left: 8px;
        }
        section {
            padding: 56px 0;
        }
        h2 {
            font-weight: 400;
            font-size: clamp(24px, 5vw, 34px);
            color: var(--gold2);
            text-align: center;
        }
        .sub {
            text-align: center;
            color: var(--mut);
            max-width: 600px;
            margin: 8px auto 30px;
        }
        .bar {
            width: 60px;
            height: 1px;
            background: var(--gold);
            margin: 12px auto;
        }
        .stats {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 10px;
            margin-top: -26px;
            position: relative;
        }
        .stat {
            background: var(--card);
            border: 1px solid var(--line);
            padding: 16px 8px;
            text-align: center;
        }
        .stat b {
            display: block;
            color: var(--gold);
            font-size: 22px;
        }
        .stat span {
            font: 12px system-ui, sans-serif;
            color: var(--mut);
        }
        .about {
            display: grid;
            gap: 22px;
            background: var(--card);
            border: 1px solid var(--line);
            padding: 26px;
        }
        .about p {
            color: #cfc9bb;
        }
        .sig {
            color: var(--gold);
            font-style: italic;
        }
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(290px, 1fr));
            gap: 20px;
            align-items: start;
        }
        .card {
            background: var(--card);
            border: 1px solid var(--line);
            overflow: hidden;
        }
        .card img {
            width: 100%;
            height: auto;
            display: block;
        }
        .cb {
            padding: 16px 18px 20px;
        }
        .tag {
            font: 11px system-ui, sans-serif;
            letter-spacing: .14em;
            text-transform: uppercase;
            color: var(--gold);
        }
        .card h3 {
            font-weight: 400;
            font-size: 19px;
            margin: 4px 0 6px;
        }
        .card p {
            color: var(--mut);
            font-size: 14.5px;
        }
        .feat {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 14px;
            margin-top: 30px;
        }
        .feat div {
            border: 1px solid var(--line);
            padding: 18px;
            text-align: center;
            background: var(--card);
        }
        .feat i, .feat svg {
            color: var(--gold);
            font-size: 22px;
            margin-bottom: 8px;
        }
        .feat h4 {
            font-weight: 400;
            font-size: 16px;
        }
        .feat p {
            font-size: 13.5px;
            color: var(--mut);
        }
        .two {
            display: grid;
            gap: 24px;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        }
        .box {
            background: var(--card);
            border: 1px solid var(--line);
            padding: 24px;
        }
        .box h3 {
            font-weight: 400;
            color: var(--gold2);
            margin-bottom: 14px;
        }
        .row {
            display: flex;
            gap: 12px;
            align-items: center;
            margin: 10px 0;
            color: var(--tx);
            text-decoration: none;
            font-family: system-ui, sans-serif;
            font-size: 14.5px;
        }
        .row i, .row svg {
            width: 20px;
            color: var(--gold);
        }
        input, textarea {
            width: 100%;
            background: #0d0d0d;
            border: 1px solid var(--line);
            color: var(--tx);
            padding: 11px;
            margin-bottom: 10px;
            font: 15px system-ui, sans-serif;
            border-radius: 2px;
        }
        input:focus, textarea:focus {
            outline: 1px solid var(--gold);
        }
        .soc {
            display: grid;
            grid-template-columns: 1fr;
            gap: 8px;
            margin-top: 6px;
        }
        .soc a {
            border: 1px solid var(--line);
            color: var(--tx);
            text-decoration: none;
            text-align: left;
            padding: 12px 14px;
            font: 13px system-ui, sans-serif;
        }
        .soc i, .soc svg {
            color: var(--gold);
            margin-right: 6px;
        }
        footer {
            border-top: 1px solid var(--line);
            text-align: center;
            padding: 26px 18px;
            color: var(--mut);
            font: 13px system-ui, sans-serif;
        }
    </style>
</head>
<body>
    <nav>
        <div class="w">
            <b>MY KÖŞK MOBİLYA</b>
            <div class="lang" role="group" aria-label="Language">
                <button type="button" data-l="tr" class="on">🇹🇷 TR</button>
                <button type="button" data-l="en">🇬🇧 EN</button>
            </div>
            <div class="lk">
                <a href="#koleksiyon">Koleksiyon</a>
                <a href="#hakkimizda">Hakkımızda</a>
                <a href="#iletisim">İletişim</a>
            </div>
        </div>
    </nav>
    <header class="hero">
        <img src="data:image/jpeg;base64,/9j/4AAQSkZJRgABAQAAkACQAAD/4QDeRXhpZgAATU0AKgAAAAgABgESAAMAAAABAAEAAAEaAAUAAAABAAAAVgEbAAUAAAABAAAAXgEoAAMAAAABAAIAAAEyAAIAAAAUAAAAZodpAAQAAAABAAAAegAAAAAAAACQAAAAAQAAAJAAAAABMjAyNjoxMDowMiAwMDowNzo1NQAABJADAAIAAAAUAAAAsJKGAAcAAAASAAAAxKACAAQAAAABAAACyKADAAQAAAABAAACywAAAAAyMDI2OjEwOjAyIDAwOjA3OjU1AEFTQ0lJAAAAU2NyZWVuc2hvdP/tADhQaG90b3Nob3AgMy4wADhCSU0EBAAAAAAAADhCSU0EJQAAAAAAENQdjNmPALIE6YAJmOz4Qn7/4gIoSUNDX1BST0ZJTEUAAQEAAAIYYXBwbAQAAABtbnRyUkdCIFhZWiAH5gABAAEAAAAAAABhY3NwQVBQTAAAAABBUFBMAAAAAAAAAAAAAAAAAAAAAAAA9tYAAQAAAADTLWFwcGwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAApkZXNjAAAA/AAAADBjcHJ0AAABLAAAAFB3dHB0AAABfAAAABRyWFlaAAABkAAAABRnWFlaAAABpAAAABRiWFlaAAABuAAAABRyVFJDAAABzAAAACBjaGFkAAAB7AAAACxiVFJDAAABzAAAACBnVFJDAAABzAAAACBtbHVjAAAAAAAAAAEAAAAMZW5VUwAAABQAAAAcAEQAaQBzAHAAbABhAHkAIABQADNtbHVjAAAAAAAAAAEAAAAMZW5VUwAAADQAAAAcAEMAbwBwAHkAcgBpAGcAaAB0ACAAQQBwAHAAbABlACAASQBuAGMALgAsACAAMgAwADIAMlhZWiAAAAAAAAD21QABAAAAANMsWFlaIAAAAAAAAIPfAAA9v////7tYWVogAAAAAAAASr8AALE3AAAKuVhZWiAAAAAAAAAoOAAAEQsAAMi5cGFyYQAAAAAAAwAAAAJmZgAA8qcAAA1ZAAAT0AAACltzZjMyAAAAAAABDEIAAAXe///zJgAAB5MAAP2Q///7ov///aMAAAPcAADAbv/AABEIAssCyAMBIgACEQEDEQH/xAAfAAABBQEBAQEBAQAAAAAAAAAAAQIDBAUGBwgJCgv/xAC1EAACAQMDAgQDBQUEBAAAAX0BAgMABBEFEiExQQYTUWEHInEUMoGRoQgjQrHBFVLR8CQzYnKCCQoWFxgZGiUmJygpKjQ1Njc4OTpDREVGR0hJSlNUVVZXWFlaY2RlZmdoaWpzdHV2d3h5eoOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4eLj5OXm5+jp6vHy8/T19vf4+fr/xAAfAQADAQEBAQEBAQEBAAAAAAAAAQIDBAUGBwgJCgv/xAC1EQACAQIEBAMEBwUEBAABAncAAQIDEQQFITEGEkFRB2FxEyIygQgUQpGhscEJIzNS8BVictEKFiQ04SXxFxgZGiYnKCkqNTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqCg4SFhoeIiYqSk5SVlpeYmZqio6Slpqeoqaqys7S1tre4ubrCw8TFxsfIycrS09TV1tfY2dri4+Tl5ufo6ery8/T19vf4+fr/2wBDAAICAgICAgMCAgMFAwMDBQYFBQUFBggGBgYGBggKCAgICAgICgoKCgoKCgoMDAwMDAwODg4ODg8PDw8PDw8PDw//2wBDAQICAgQEBAcEBAcQCwkLEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBAQEBD/3QAEAC3/2gAMAwEAAhEDEQA/AP5/6KKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA/9D+f+iiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKAP/R/n/ooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigD/0v5/6KKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA/9P+f+iiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKAP/U/n/ooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAoopcHr60AJRTtj7PM2nYDjOOM+mabQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAf/9X+f+iiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKUAsQo6nigBKKKKACiiigAp7hAF2MSSPm4xg5PHvxSuYyqbFIIHzZOcnJ5Hpxio6ACpGmkeNImYlI87R6Z61HRQAu5tu3PHXHbNJTgE2kknd2FIAScAZoASiiigAooooAcVYAMQQG6H1ptOLMVCk5C9B6U2gAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA/9b+f+iiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKe0juFVjkINo9hkn+ZoAZRRRQAVII8xNLuUbSBtPU59KjooAKKKKACiiigAooooAKKKKACiitrw/oGreJ9XtdD0S1levLy8kWOOKJdzMzHGAP8AIHek2krsaTbsjFor7L8S/smapo3giHTbF+brr3Ifisghz0KjV3Y80qZSpK9h4ooxRXZfscQYp8UksMqyROUdSCCpwQR0INV6KANrw/oGreJ9XtdD0S1levLy8kWOOKJdzMzHGAP8AIHek2krsaTbsjFor7L8S/smapo3giHTbF+brr3Ifisghz0KjV3Y8vP7MvxejuJLb/AIRuVvKxl1ZCpycHDByDj0oVSk9pITpVF0Z8v0UrKUYqeCOKTFWYhRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQAUUUUAFFFFABRRRQB//1v5/6KKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooA/9n/+IMWElDQ19QUk9GSUxFAAEBAAAMSExpbm8CEAAAbW50clJHQiBYWVogB84AAgAJAAMAMwAaYWNzcEFQUEwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA9tYAAQAAAADTLUxpbm8AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAtkZXNjAAABUAAAAEljcHJ0AAABXAAAADx3dHB0AAABaAAAABRydGVhAAABfAAAAAZjaGFkAAABkAAAACxyVFJDAAABpAAAAAtnVFJDAAABpAAAAAtiVFJDAAABpAAAAAtkZXNjAAAAAAAAAB1HZW5lcmljIFJHQiBQcm9maWxlIC0gc3RhbmRhcmQgUkdCIFByb2ZpbGUAAAAAAAAAAAAAAB1HZW5lcmljIFJHQiBQcm9maWxlIC0gc3RhbmRhcmQgUkdCIFByb2ZpbGUAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAG1sdW
