# EDEK WWW — iteracja koncepcyjna v1.2 (2026-10-28)

## Kontekst
Feedback po v1.1: biały znak E nie miał własnej tożsamości; jaskrawe kody kolorów bez kontrolowanego blasku nie wyglądały na neonowe; nie było jasne, który język strony jest aktywny; mieszane polsko-angielskie nagłówki utrudniały ocenę przekazu; prezentacja nie odzwierciedlała struktury i filarów projektu.

## Zmiana v1.2
- Znak E ma autorski holograficzno-pryzmatyczny gradient limonka → turkus → fiolet → róż. Monogram pozostaje propozycją projektu, nie zastępuje z automatu oficjalnego pliku logo.
- Neonowe barwy to nie tylko HEX: glow, drop-shadow, punktowe światła i akcenty na ciemnym tle; priorytet limonki `#CCFF00`. Wewnętrzne akcenty: `#00FFDF` turkus, `#E13BFF` fiolet, `#FF305D` czerwień. Szafir `#436AFF` pozostaje tylko kontekstowym wyróżnikiem persony edek; nie stanowi dodatkowej dominującej warstwy.
- Konsekwentny język główny PL oraz prawdziwe przełączenie PL/EN dla wszystkich nagłówków, sekcji, opisów, przycisków, nawigacji, tekstów dostępności i podstawowych metadanych. Własne nazwy utworów i EDEK pozostają niezmienne.
- Pełniejsze odzwierciedlenie IA: hero marki, trzy persony, próbka katalogu (linki odziedziczone z publicznego repo, do weryfikacji), projekt niezależny Roots & Craft wyraźnie odróżniony od rzeczywistej współpracy, trzy zastosowania B2B, transparentny opis procesu AI, o mnie, kontakt i social.
- Grafika główna (hologram E) w CSS; nie opiera widoku na stockach ani cudzych znakach.
- Rzeczywiste interakcje: sekcje kotwicowe, menu mobilne, PL/EN, linki platform (pochodzą z aktualnego pliku main). Nie ma atrap odtwarzaczy ani udawanych linków do klientów.

## QA (Chromium, widok lokalny)
- Desktop: 1440 × 920, mobile: 390 × 844 — render + pełne zrzuty, brak poziomego overflow.
- PL/EN: nagłówek, menu, hero, opisy, tytuł i meta description zmieniają język; przełączenie powrotne działa.
- Menu mobilne: otwarcie/zamknięcie i automatyczne zamknięcie po kliknięciu kotwicy.
- Brak błędów JavaScript w scenariuszach testowych.
- Przetestowano 84 elementy przetłumaczalne; tytuły utworów są nazwami własnymi.
- Nie wykonano Lighthouse/WCAG 2.2 AA, audytu praw autorskich ani aktualnej weryfikacji URL YouTube/Social.

## Uwagi krytyczne przed wdrożeniem
1. `preview-v2/index.html` to prototyp UX, bez prawdziwej synchronizacji z katalogiem i zapleczem administracyjnym.
2. Nie publikować jako strony produkcyjnej bez zatwierdzenia logo, tekstów, linków, danych utworów, kontaktu i prawnego minimum.
3. Zweryfikować, czy istniejący plik logo `edek_logo.svg` ma być bazą oficjalnej identyfikacji; obecny holograficzny E jest eksploracją jego roli wizualnej, a nie decyzją prawno-markową.
4. Nieweryfikowane firmy i nieukończone utwory pozostają wyłącznie neutralnymi koncepcjami. Nie udawać kampanii.
5. Po decyzji kierunkowej wdrażać stronę v2 zgodnie z WWW Project Master (lekki frontend, assety, SEO, pełne podstrony), poza main aż do QA.

## Status
Propozycja v1.2 oczekująca na ocenę wizualną. Production main pozostaje nienaruszone.
