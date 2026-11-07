# EDEK WWW v2 — REJESTR DECYZJI I PLAN KONTROLOWANEGO WDROŻENIA
Data aktualizacji: 2026-11-07
Właściciel wizji i zatwierdzający: użytkownik / EDEK. Koordynacja analizy, rekomendacji i technicznego wdrożenia: ChatGPT w granicach dostępnych narzędzi i zgód. Nie udawać zewnętrznego CEO ani nie uznawać hipotez za zgodę klienta.
Status: PROJECT GOVERNANCE v1.0 — obowiązuje w dalszych pracach WWW v2. Nie nadpisuje kanonu Brand & Business Decision ani Master dokumentów domenowych.

## I. Zweryfikowany stan techniczny
- Repozytorium: ededeedek/edek; prod/main pozostaje niezmieniony.
- Draft PR #2 https://github.com/ededeedek/edek/pull/2
- Gałąź: design/edek-neon-legibility-v1-1
- Prototyp: preview-v2/index.html; asset: preview-v2/assets/edek-speaker-logo.webp
- Etap 1: logo głośnikowe, logo EDEK bez kropki, napis ed • ede • edek, neonowe orbity i PL/EN — zaimplementowane w prototypie i testowane lokalnie, NIE opublikowane.
- YouTube: kanał @ed-ede-edek, banner z jedną centralną twarzą i dwiema kolorowymi sylwetkami ed/ede/edek oraz napisem EDEK; grafiki udostępnione w rozmowie, nie pełne archiwum kanału.
- VidIQ potwierdził powiązany kanał, ale limit kredytów uniemożliwił pobranie pełnego katalogu w bieżącym wywołaniu. Nie udawać kompletnego audytu 104 filmów.
- Osobna przeglądarka Mac nie jest dostępna z kontekstu iPhone'a; nie zakładać nieograniczonego zdalnego dostępu.

## II. Decyzje strategiczne — FROZEN
1. EDEK to jedna marka artystyczna z energiami ed, ede, edek; nie są trzema samodzielnymi markami.
2. Publiczna witryna ededeedek.pl jest centrum marki i portfolio; YouTube pozostaje głównym kanałem odsłuchu.
3. Design premium: dominują ciemne tła, limonka #CCFF00 jako kod nadrzędny, kontrolowane neonowe turkus/fiolet/czerwień, szafir istnieje w tożsamości persony edek. Nie używać wszystkich kolorów na raz w każdej sekcji.
4. Logo głośnikowe edek jest wyróżnikiem muzycznym w nagłówku i hero; lockup EDEK bez kropki + „ed • ede • edek”; bez kolejnych nieuzgodnionych redesignów.
5. WWW PL jako język domyślny + rzeczywisty, kompletny EN. Slogany własne mogą zostać po angielsku tylko, jeśli celowo zapisane jako nazwy; bez przypadkowej mieszanki.
6. EDEK for Brands to jedna podsekcja usługowa (hipoteza biznesowa do weryfikacji), nie udawana agencja z portfolio klientów.
7. „Koncepcja inspirowana” != „współpraca z firmą”. Nie używać logo, wizerunków, nazw jako reklamy, jeśli nie zweryfikowano praw i granic zastosowania.

## III. Pomysły z burzy mózgów — DECYZJA
- Baner YouTube: zachować jako referencję wizualną, nie wklejać 1:1 jako hero. Wizerunek centralny i dwie wersje kolorystyczne to unikalny motyw marki.
- Miniatury: audyt jakości i praw, następnie użycie wybranych rzeczywistych miniaturek jako kart utworów. Nie zastępować miniaturek generowanymi abstrakcjami.
- EDEK Mode Switch: PRZYJĘTY JAKO HIPOTEZA UX DO PROTOTYPU w sekcji „Trzy energie” poniżej hero, nie jako zamiana logo. Kliknięcie/tap wybiera personę, zmienia narrację, zdjęcie, kolor i filtr utworów. Bez autoplay i bez automatycznej zmiany całego motywu strony; zachować dostępność, reduced motion i lekkość.
- Zakazane na obecnym etapie: dodatkowe interaktywne gadżety, 3D obciążające mobile, osobny kanał WWW dla każdej persony, kosmetyczne redesigny bez problemu użytkownika, niezweryfikowane statystyki i referencje.

## IV. Kolejność prac i bramki jakości
ETAP 1 — Design System/logo/hero: technicznie wykonany na branchu, wizualnie zaakceptowany w rozmowie; bez publikacji.
ETAP 2A — AUDYT ASSETÓW I KATALOGU, TERAZ:
  1. Zebrać udostępniony baner, zasoby GitHub oraz okładki/miniatury dostępne legalnie w projekcie i zweryfikowanych kanałach.
  2. Oznaczyć każdy asset: właściciel/prawa, persona, utwór, data, format i docelowe miejsce na stronie.
  3. Wybrać reprezentatywne 6–9 utworów dopiero po sprawdzeniu danych źródłowych, a następnie określić kolejność, CTA i opisy.
  4. Rezultat: kanoniczna mapa assetów i lista realnego katalogu. Bez udawania pełnego audytu, jeśli dane są niekompletne.
ETAP 2B — IA i UX:
  1. Home: hero z logo → trzy energie z Mode Switch → wybrane utwory → sekcja for Brands → AI w praktyce → o mnie → kontakt/social.
  2. Podstrony/kategorie: Muzyka, Dla marek, Proces/AI, O mnie, Kontakt oraz niezbędne legal pages.
  3. Każde CTA ma prawdziwy cel. Dostępność i wydajność mobile są bramkami, nie dodatkami.
ETAP 3 — Content i integracje: wyłącznie zweryfikowane YouTube, TikTok, IG, Facebook; bez wymyślonych linków; embed z uwzględnieniem prywatności i wydajności.
ETAP 4 — prawo i monetyzacja: weryfikacja licencji Suno/audio/grafik, prawo do wizerunku/znaków towarowych, transparentne oznaczanie koncepcji vs kampanii, prosta oferta B2B. Potwierdzenie popytu przed cennikiem.
ETAP 5 — QA, SEO, mobile, WCAG, publikacja po zatwierdzeniu; bez merge do main przed przejściem bramek.

## V. Reguły zarządzania
- Każdy pomysł klasyfikować: DECYZJA / HIPOTEZA DO TESTU / BACKLOG / ODRZUCONY.
- Zmiana istniejącego założenia wymaga wskazania problemu, wpływu na markę, kosztu i decyzji właściciela.
- Jeden aktywny etap naraz; nie przeskakiwać w konfigurację social przed audytem źródła (YouTube).
- W każdym checkpointcie podawać: wykonano / blokery / następny krok / czy ruszono produkcję.
- Prototyp i grafika referencyjna to nie strona produkcyjna. Rozróżniać tworzenie mockupów od implementacji HTML i wgrania do repo.
- Nie sugerować, że coś zapamiętano w systemowej pamięci po samej wypowiedzi: status zapisujemy w PROJECT MASTER i repozytorium.

## VI. Następna konkretna czynność
Zamknąć ETAP 2A: audyt dostępnych zasobów bannera i rzeczywistych miniaturek (najpierw repo/Library, potem dalsza weryfikacja katalogu YouTube gdy będzie dostępna). Przygotować tabelę asset → persona → potencjalny moduł WWW i 1 ekran demonstracyjny Mode Switch na istniejących wizerunkach. Bez zmian na main.
