# EDEK WWW — audyt repozytorium i korekta identyfikacji v1.1
Data: 2026-10-28
Repozytorium: ededeedek/edek
Baza audytu: main (GitHub REST, odczyt plików) + istniejąca gałąź dev-preview + dokumenty nadrzędne EDEK (Brand & Business Decision v1.0, Visual System, EDEK.PL V2 Project Master).
Zmiana: nowa propozycja widoku w preview-v2/index.html, BEZ modyfikacji index.html produkcyjnego i BEZ wdrożenia.

## 1. Fakty zweryfikowane
- `main/index.html` to pojedynczy plik HTML ~28 KB, który ładuje React 18 development, ReactDOM development, Babel Standalone i Tailwind CSS z CDN; JSX jest transpILowany w przeglądarce.
- `main` zawiera 13 ręcznie wpisanych rekordów w `musicDatabase`. Nie są synchronizowane automatycznie z YouTube.
- Obecne akcenty na `main`: `#22c55e` (ed), `#ef4444` (ede), `#3b82f6` (edek); dodatkowo lokalny fiolet w klasach Tailwind.
- Istniejąca odrębna gałąź `dev-preview` używa `#00e5ff` (cyan) oraz `#ff2dff` (magenta). To nie jest dowód, że te barwy są używane na produkcji.
- Na `main` nagłówek pokazuje „ED EDE EDEK”, hero „LEKARSTWO MUZYCZNE”, a stopka ma rok 2025, pozorne linki `href="#"` dla regulaminu i polityki prywatności oraz odznakę `Certified Human & AI Hybrid Art`.
- W repo są m.in. `logo.PNG`, `edek_logo.svg` i istniejące avatary. Nie założono, że dowolny z tych plików można bez oceny używać jako nowego oficjalnego znaku.
- Publiczna strona korzysta z domeny ededeedek.pl, a statyczna witryna jest w repo `ededeedek/edek`. Wersja w `main` nie zawiera jeszcze architektury `/muzyka`, `/ai`, `/produkty`, `/o-mnie`, `/kontakt` wymaganej w docelowym WWW v2.

## 2. Ryzyka i rekomendowane priorytety
### P0 — przed publikacją v2
1. Utrzymać EDEK jako nazwę główną (trzy persony ed • ede • edek pozostają językiem kreatywnym).
2. Usunąć pozorne „certyfikaty”, nieweryfikowane wyniki i niezweryfikowane portfolio klientów.
3. Zastąpić martwe linki regulaminu/polityki prawdziwymi stronami lub nie pokazywać ich jako działających odnośników.
4. Przed umieszczeniem logotypów, nazw firm, wizerunków i reklam uzyskać właściwe uprawnienia; projekt autorski musi pozostać odróżniony od rzeczywistej współpracy.
5. Potwierdzić licencje audio/grafik i zasady dostępu do materiałów.

### P1 — jakość serwisu i marka
1. Zastąpić dev React/Babel/Tailwind CDN wdrożeniem lekkim, statycznym z kompilacją build-time; zgodnie z WWW Project Master preferowane Vite + TypeScript/JS + CSS.
2. Rozdzielić bazę katalogu muzycznego od warstwy prezentacji; nie publikować niezweryfikowanych linków.
3. Uzupełnić SEO: title/description/canonical/OG, poprawne ikony, sitemap, robots, metadane dla kart utworów.
4. Poprawić semantykę HTML, dostępność klawiatury, responsywność, kontrast i preferencję reduced-motion.
5. Docelowe podstrony oraz przejścia social oprzeć o stan potwierdzonych profili.

### P2 — optymalizacja
1. Skompresować ciężkie assety i ocenić LCP/CLS/INP na rzeczywistym wdrożeniu.
2. Uruchomić pomiar przejść do muzyki i zapytań o współpracę, bez przedwczesnego rozbudowywania narzędzi.
3. A/B testować komunikat i rodzaj grafik dopiero po dostępie do danych.

## 3. Korekta Design System v1.1 — propozycja, jeszcze nie zatwierdzony kanon
| Token | Kolor | Funkcja |
| --- | --- | --- |
| Background | #0A0A0A | Tło główne |
| EDEK Lime | #CCFF00 | Główny sygnał marki i CTA |
| Neon Turquoise | #00F5D4 | Linie i świetlne cyfrowe akcenty |
| Fluorescent Violet | #DA37FF | Akcent eksperymentalny/glitch |
| Signal Red | #FF335A | Energia ede / punktowy akcent |
| Sapphire Blue | #4978FF | Głębia, edek i wybrane materiały |
| Primary text | #F4F6F3 | Tekst |
| Secondary text | #A5ACB1 | Opisy i metadane |

Zasada: większość powierzchni pozostaje czarno-grafitowa. Limonka prowadzi interakcję; turkus, fiolet i czerwień występują jako rozproszone akcenty, a nie wielokolorowa poświata wokół wszystkiego. Kolory nie zastępują sensu utworu ani istniejącego kanonu person.

## 4. Czytelność znaku i nagłówka
- Stary mały zapis ED[E]K miał nadmiernie ścieśnione litery; nowy lockup: kontrastowy monogram E + pełny napis EDEK. + podpis ed • ede • edek.
- W hero litera E jest prosta (bez obrotu), biała i pozbawiona nakładających się opisów. Obok/pod spodem występuje pełna nazwa EDEK.
- Outline słowa STORIES zamieniono na pełne krycie. Wielkość hero dopasowano do telefonu.
- Monogram E w prototypie to **propozycja aplikacji graficznej**, nie ogłoszenie zastąpienia dotychczasowego oficjalnego logo.

## 5. Zakres prototypu i test
- Plik `preview-v2/index.html` to oddzielny statyczny projekt UX/UI, nie działający katalog muzyczny i nie oficjalna oferta B2B.
- Rzeczywiste linki YouTube/TikTok/Instagram pochodzą z publicznego kodu repozytorium; ich aktualnego statusu logowania, właścicielstwa i profili nie potwierdzono osobno.
- Sekcje portfolio są wyraźnie nazwane koncepcjami ilustracyjnymi, nie istniejącymi kampaniami ani referencjami.
- Lokalnie przetestowano renderowanie w Chromium dla 1440 px i 390 px: brak poziomego overflow; menu mobilne otwiera się i zamyka po wybraniu sekcji.
- Test nie obejmuje produkcyjnego Lighthouse, dostępności pełnego WCAG, aktualności profili social ani poprawności wszystkich linków.

## 6. Zasada wdrożenia
`main` pozostaje nienaruszony. Przed wdrożeniem: ocenić i zatwierdzić kierunek v1.1, zasoby graficzne, mapę treści, dane utworów, prawne strony i przełączniki językowe. Następnie implementować w oddzielnym branchu i przeprowadzić QA przed merge.
