# EDEK WWW v2 — kontrola jakości raportu AI z YouTube Studio
Data: 2026-11-07. Źródło: pełny tekst raportu AI YouTube Studio wklejony przez właściciela projektu w rozmowie. Dane to deklaracje raportu, a nie zweryfikowany odczyt API z tej rozmowy.

## Rzeczywiście otrzymano
- Raport deklaruje: 104 publiczne materiały, 32 długie filmy, 72 Shorts.
- W przekazanej tabeli głównych publikacji jest jednak **41 wierszy oznaczonych Film**, w okresie 2025-10-29 do 2026-10-30.
- Tabela zawiera pełne/niemal pełne tytuły, 11-znakowe identyfikatory filmów, daty, czasy, wyświetlenia, polubienia, komentarze, CTR, średni procent obejrzenia; pole miniaturek NIEDOSTĘPNE.
- Załączone wcześniej zrzuty mobilnego YouTube są osobnym potwierdzeniem aktualnego widoku części miniaturek, ale nie identyfikatorów wideo.
- Zewnętrzna strona TopAIMuza pokazuje 37 utworów zakwalifikowanych do własnego katalogu na 2026-11-04. To NIE dowodzi, że kanoniczny kanał YouTube ma 37 filmów.

## Blokery wiarygodności danych
1. **32 vs 41**: jawna sprzeczność między deklarowaną liczbą filmów długich i liczbą pozycji w tabeli. Wymagane wyjaśnienie filtra.
2. **COUNT THE FEW**: dane wejściowe (1576 wyświetleń * 243 sekundy * 0,2728) dają ~29,0 h czasu odtwarzania, a raport rankingu watch time podaje 21 h 26 min. Metryki mogą mieć inny zakres dat lub definicję — nie rozstrzygaj bez źródeł.
3. **BILANS**: podpis „w pierwszych 8 dniach” przy wydaniu z 2026-07-13 w raporcie sporządzonym 2026-11-07 wymaga objaśnienia okresu i jego granic.
4. **Rozbieżności z publicznym YouTube**: np. wzrost 116→118 MÓJ CZAS może wynikać z czasu odczytu, ale inne różnice (CODE ZERO 21 vs 44; GAZZZOLINA 50 vs 104 na wcześniejszym screenie) są zbyt duże, aby bez potwierdzenia traktować je jako ten sam zakres liczenia.
5. **TOP CTR**: brak liczby impressions, więc wysoki CTR przy małej próbie może być niestabilny; nie obiecywać wyników poprzez samo kopiowanie miniatury.
6. **Retencja**: średni procent obejrzenia nie jest bezpośrednio porównywalny między 1:40, 4:57 i 22:20 bez kontekstu czasu trwania; SYSTEM FLOW wymaga osobnej kategorii.
7. **Miniatury**: URL nie został dostarczony, oficjalny wariant potwierdzamy wizualnie z YouTube lub źródłem YouTube, nie przez automatyczny wybór lokalnej grafiki.

## Decyzja projektowa
Status **PROVISIONAL / NIE IMPORTOWAĆ BEZ KONTROLI**. 41 pozycji jest roboczym katalogiem do walidacji; nie uznawać 32/72 jako wiążących. Listy TOP i rekomendowanych 9 traktować jako hipotezę redakcyjną. Nie wprowadzać statystyk na publiczną stronę WWW. Nie zmieniać main.

## Wstępne zestawienie 9 rekomendowanych w raporcie (NIE finalna selekcja)
| Video ID | Tytuł skrócony | Publiczny odsyłacz |
|---|---|---|
| vlSTVeicCUw | Dopóki lecimy | https://www.youtube.com/watch?v=vlSTVeicCUw |
| XjevEYJzNMI | COUNT THE FEW | https://www.youtube.com/watch?v=XjevEYJzNMI |
| aDkHX82o3Us | NOWA ERA | https://www.youtube.com/watch?v=aDkHX82o3Us |
| TNOzKsX4G6s | DRIFT i BASS | https://www.youtube.com/watch?v=TNOzKsX4G6s |
| QZwwUdKfJv4 | Rozbijam ten mur | https://www.youtube.com/watch?v=QZwwUdKfJv4 |
| t-kKWCq9RhA | CODE ZERO | https://www.youtube.com/watch?v=t-kKWCq9RhA |
| gg4phNAITxM | GAZZZOLINA | https://www.youtube.com/watch?v=gg4phNAITxM |
| _-LlKmbLaC0 | MÓJ CZAS | https://www.youtube.com/watch?v=_-LlKmbLaC0 |
| QVRBj_1hWtk | Zgubiłem się w Twej pamięci | https://www.youtube.com/watch?v=QVRBj_1hWtk |

## Następny krok
Jedno zadanie korekcyjne dla AI Studio: policzyć 41 pozycji, wyjaśnić 32 vs 41; ujednolicić zakres dat/definicję wyświetleń, CTR i czasu oglądania; ponownie zweryfikować COUNT THE FEW; poprawić BILANS; zwrócić brakujące utwory lub wyraźnie uzasadnić filtr; bez ponownej rozbudowanej rekomendacji SEO.