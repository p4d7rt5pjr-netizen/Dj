# 🎧 AI DJ Party — PWA

Wirtualny DJ z AI, który puszcza Twoją muzykę i komentuje jak prawdziwy wodzireJ.

## 📁 Pliki

```
index.html   ← główna aplikacja
manifest.json ← konfiguracja PWA
sw.js        ← service worker (tryb offline)
icon-192.png ← ikona aplikacji
icon-512.png ← ikona aplikacji (duża)
```

## 🚀 Jak uruchomić na iPhone

### Opcja 1: GitHub Pages (zalecana, darmowa)

1. Utwórz konto na https://github.com
2. Utwórz nowe repozytorium (publiczne)
3. Wrzuć wszystkie pliki z tego folderu
4. Wejdź w Settings → Pages → Source: main branch
5. Poczekaj 2 minuty — strona będzie pod adresem:
   `https://TWOJA_NAZWA.github.io/NAZWA_REPO/`
6. Otwórz ten adres w Safari na iPhone
7. Dotknij przycisku Udostępnij ↑ → "Dodaj do ekranu głównego"
8. Gotowe! Masz aplikację na ekranie głównym 🎉

### Opcja 2: Netlify Drop (najszybsza)

1. Wejdź na https://app.netlify.com/drop
2. Przeciągnij i upuść cały folder `dj-pwa`
3. Otrzymasz link — otwórz go w Safari na iPhone
4. Safari → Udostępnij ↑ → "Dodaj do ekranu głównego"

### Opcja 3: Lokalny serwer (dla developerów)

```bash
cd dj-pwa
python3 -m http.server 8080
# Otwórz http://localhost:8080 w przeglądarce
```

## ⚠️ Ważne dla iOS

- iOS wymaga **HTTPS** dla PWA (GitHub Pages i Netlify dają HTTPS automatycznie)
- Audio może pauzować gdy ekran się wygasi — to ograniczenie Safari na iOS
- Testowane na iOS 16+

## 🎛️ Funkcje

- 4 osobowości DJ-a (Hype, Smooth, Retro, Festival)
- Komentarze AI generowane przez Claude
- Regulowane przerwy między utworami (3-30s)
- Tryb shuffle
- Własne pliki muzyczne (MP3, WAV, OGG, FLAC, M4A)
- Działa offline po pierwszym załadowaniu
