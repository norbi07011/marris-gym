# Marris Gym · Sportcentrum Den Haag

Nowa strona Sportcentrum Marris Gym (Mangaanstraat 50, 2544 DW Den Haag): kickboxing, boks tajski, Taekwon-Do (ITF), Women Only, Polska Grupa, siłownia i trening personalny.

## Co jest w środku

| Plik / folder | Zawartość |
| --- | --- |
| `index.html` | Cała strona w jednym pliku: style, skrypty, tłumaczenia NL / PL / EN i zdjęcia (osadzone w pliku). |
| `media/` | Filmy: rolki ze strony głównej (`reel*.mp4` + krótkie podglądy i okładki) oraz film w karcie Siłownia (`fitness.mp4`). |

Strona działa bez budowania i bez serwera aplikacji. Wystarczy dowolny hosting plików statycznych.

### Podstrony (nawigacja przez `#`)

- `#home`: worek 3D, rolki, zapowiedź Legion Octagon Academy, Aleja Gwiazd, Cancer Fighters, reklama Fit Diet
- `#lessen`: zajęcia (7 kart)
- `#rooster`: grafik z filtrem grup i godziny siłowni
- `#tarieven`: cennik
- `#kinderfeest`: urodziny dla dzieci
- `#partners`: partnerzy (Fit Diet Catering, King Protein, Octagon Sport NL)
- `#contact`: formularz wysyłany przez WhatsApp (Kuba po polsku / Stefan po niderlandzku) i mapa 3D

### Biblioteki zewnętrzne (CDN)

- three.js r128 (worek 3D, mapa 3D)
- GSAP 3.12.2 + ScrollTrigger (animacje)
- Google Fonts: Big Shoulders Display, Archivo, JetBrains Mono

## Podgląd lokalny

Filmy ładują się ze ścieżek względnych, więc najlepiej uruchomić prosty serwer w folderze repozytorium:

```bash
python3 -m http.server 8000
# potem otwórz http://localhost:8000
```

## Publikacja na GitHub Pages

1. W repozytorium: **Settings → Pages**.
2. Source: **Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Po chwili strona będzie dostępna pod adresem `https://norbi07011.github.io/marris-gym/`.

Własną domenę (np. `marrisgym.nl`) można podpiąć w tym samym miejscu w polu **Custom domain**.
