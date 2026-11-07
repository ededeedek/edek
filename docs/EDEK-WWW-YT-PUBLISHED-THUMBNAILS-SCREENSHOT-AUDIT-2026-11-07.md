# EDEK WWW v2 — publiczne miniatury kanału / audyt ze zrzutów YouTube
Data: 2026-11-07
Źródło: sześć zrzutów ekranu dostarczonych przez użytkownika z mobilnej aplikacji YouTube, zakładka Wideo, sortowanie "Najnowsze", filtr "Publiczny". Nie jest to zrzut pełnego katalogu ani dostęp do YouTube Studio API.

## Cel
Odróżnienie rzeczywistych miniaturek widocznych przy opublikowanych filmach od wielu wariantów powstających w ChatGPT Library. Te zrzuty są referencją dla obecnego stanu publikacji, a nie alternatywnymi grafikami do odtworzenia.

## Rekordy, które można jednoznacznie odczytać wzrokowo
| Widoczna nazwa / skrót | Pasek miniatury | Cechy | Ograniczenia |
|---|---|---|---|
| Edek – MÓJ CZAS | czerwony | twarz na tle biuro/dom; napis MÓJ CZAS | tytuł po `Polski Blues-Rock...` ucięty |
| Edek – Nie poganiaj mnie | czerwony | siedzący portret w pomieszczeniu, bez wielkiego tytułu | końcówka tytułu ucięta |
| A Twoje Dziecko Robi SIX-SEVEN? | limonka | scena rodzinna, napis SIX-SEVEN? na dole | końcówka tytułu ucięta |
| CODE ZERO | czerwony | portret, napis CODE ZERO | końcówka tytułu ucięta |
| TEREFERE MORDO — sok za sokiem | limonka | postać z napojem, duży napis neonowy | końcówka tytułu ucięta |
| PRAWIE | szafir/niebieski | postać w czarnym stroju, napis PRAWIE | pełny tytuł nieznany |
| EDEK STYLE — kiedy glitch przej... | limonka | postać na zielono-fioletowym klubowym tle | końcówka tytułu ucięta |
| COUNT THE FEW | czerwony | ciemny korytarz i portret | końcówka tytułu ucięta |
| Z rozpędu w przepaść | szafir | jazda nocą, portret w aucie | pełny tytuł ucięty |
| PRZECIĄŻENIE — za mocno? Tak ma by... | limonka | DJ w świetle fioletowo-niebieskim | nie utożsamiać z inną grafiką OVERLOAD z czerwonym paskiem |
| GAZZZOLINA — polski reggaeton... | limonka | dynamiczna postać w industrialnej scenerii | tytuł ucięty |
| Dałem wszystko. Więcej już nie mo... / BILANS | czerwony | ciemna narracyjna scena, napis BILANS | tytuł ucięty |
| DOPAMINE OVERDOSE | czerwony | dwa portrety w ciemnym otoczeniu | dalszy ciąg tytułu ucięty |
| SUPER-MEM | szafir | portret na tle zachodu / czerwonej peleryny | pełny tytuł ucięty |
| Ten numer zresetuje Ci głowę... | limonka | twarz, kolorowy stworek, napis WCHODZISZ? | pełny tytuł ucięty |
| The Architect | czerwony | industrialny korytarz, portret, pozioma czerwona linia | dalszy tytuł ucięty |
| Jadę swoją drogą | szafir | jazda autem w nocy z elementem widma | dalszy tytuł ucięty |
| Nie uniosłaś | szafir | gramofon i portret w środku | dalszy tytuł ucięty |
| Italy in April: Puglia Storm | niebiesko-żółty | fale/Polignano a Mare; duże litery PUGLIA IN APRIL | czy persona z paska nie wynika jasno |
| SYSTEM FLOW / 100% FOCUS | wielokolorowy | neonowa scena; 22:20, dłuższy format | nie klasyfikować automatycznie jako zwykłego singla |
| Ta Noc | szafir | postaci i duża typografia TA NOC | dalszy tytuł ucięty |
| Raz w Roku | szafir | dwie postaci, zachód słońca | dalszy tytuł ucięty |
| BEZ IMION | szafir | dwie sylwetki, gradient róż/niebieski | dalszy tytuł ucięty |
| PROTOKÓŁ 562 | szafir | futurystyczna jazda nocą, napis PROTOKÓŁ 562 | dalszy tytuł ucięty |
| SZKLANY DOM | szafir | ekspresyjny portret, pęknięte szkło | dalszy tytuł ucięty |
| NOWA ERA | czerwony | samochód i postać, rozdzielenie błyskawicą | dalszy tytuł ucięty |
| LAST CHRISTMAS ALE TO BIGOS | limonka | świąteczna kompozycja | pełny tytuł ucięty |
| Świąteczny KLIMAT i SPOKÓJ | szafir | trzy postacie w strojach świątecznych | końcówka tytułu ucięta |
| Szybki DRIFT i BASS / EDE MO... | czerwony | czerwone auto i edek CLUB | pełny tytuł ucięty |
| Agresywna ENERGIA / EDE... | czerwony | trzy postacie na klubowej scenie | pełny tytuł ucięty |
| Mega Świnia / Brawl Stars | limonka | grafika gry z napisem | pełny tytuł ucięty |

## Wnioski potwierdzone
- Zrzuty pokazują aktualnie prezentowane miniatury i ich widoczne typy; nie są jedynie obrazami źródłowymi z biblioteki.
- Identyfikacja wielu materiałów realizowana jest poprzez pionowy pasek na lewej krawędzi w limonce, czerwieni lub szafirze, ale bez pojedynczego nieomylnego algorytmu przypisywania persony.
- Miniatury są stylistycznie zróżnicowane: duży tekst, filmowy portret, scena tematyczna albo ilustracja fantastyczna.
- Dla modelu WWW: miniatura rzeczywistego filmu ma pierwszeństwo nad plikiem podobnym wizualnie z Library.
- „MÓJ CZAS” to publikacja tak nazwana na kanale; plik Library nazwany Moje Tempo wymaga korekty mapowania, nie automatycznej zmiany nazwy samego pliku.
- „PRZECIĄŻENIE” widoczne na YouTube ma limonkowy pasek; obraz „OVERLOAD” w Library z paskiem czerwonym to inny motyw/wersja. Nie wolno utożsamiać bez dowodów.

## Krytyczne luki
- Zrzuty nie ujawniają ID filmów, bezpośrednich URL, pełnych opisów i wszystkich tytułów.
- Nie dowodzą, że konkretny PNG Library ma identyczną wersję bitmapy jak na kanale — potwierdzają wizualne podobieństwo.
- Nie należy kopiować miniatur ze zrzutów jako grafik WWW, ponieważ mają mniejszą rozdzielczość i zawierają UI aplikacji.
- Nie ma podstaw do rankingu CTR na podstawie samej liczby wyświetleń lub estetyki zdjęcia.

## Decyzja wdrożeniowa
Przygotować manifest filmów z kluczami video ID, pełny tytuł i thumbnail URL z YouTube (po wiarygodnym pozyskaniu), a dla 6-9 rekomendowanych wydań dopasować grafiki z Library wyłącznie po rozpoznaniu aktualnej wersji na kanale. Nie wprowadzać żadnych zmian w main.