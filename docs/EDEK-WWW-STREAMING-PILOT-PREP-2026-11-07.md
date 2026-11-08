# EDEK — przygotowanie do pilotażu dystrybucji (bez zakupu usługi)

Decyzja właściciela projektu z 2026-11-07: przygotowania Spotify prowadzić równolegle z WWW, bez zakupu abonamentu ani aktywowania płatnej usługi.

## Status
Pomysł biznesowy przyjęty do roadmapy; brak potwierdzenia, że podpisano umowę z dystrybutorem lub opublikowano wydanie. Nie wybierać dostawcy bez aktualnego przeglądu cen i zasad dystrybucji materiałów generowanych z AI.

## Zakres prac bez kosztu
1. Zbudować listę 2–3 możliwych utworów pilotażowych. Nie uznawać utworu automatycznie za gotowy prawnie.
2. Karta praw dla każdego: autorstwo tekstu, źródło kompozycji/audio i głosów, użyte narzędzie i rodzaj planu/subskrypcji w momencie tworzenia, warunki licencji, źródło grafiki, wykorzystane próbki i remiksy.
3. Karta plików: master audio (format/parametry), okładka, artysta EDEK, dokładny tytuł, wykonawcy i współautorzy, data planowana, język, treści wymagające oznaczeń.
4. Porównanie potencjalnych agregatorów: zgodność z regulaminami AI, własność mastera i identyfikatorów, prowizje i opłaty, ryzyko usunięcia katalogu po rezygnacji, YouTube Content ID (ważne dla istniejących filmów), mechanizm wypłat, podatki i rozliczenia, możliwość korekty metadanych.
5. Po kwalifikacji materiału: utworzyć identyfikatory artysty i wydania oraz zapisać je w kontrolowanym rejestrze.
6. Dopiero po potwierdzeniu opublikowanego wydania odblokować linki Spotify/Apple Music/YouTube Music na WWW.

## Kryteria decyzji GO / NO-GO
GO wyłącznie gdy: udokumentowane prawa, format i mastering zgodny z dystrybutorem, koszty zaakceptowane, brak konfliktu Content ID i spójne metadane. NO-GO: niewyjaśnione prawa do utworu/remiksu/próbek/obrazów lub opłaty niezaakceptowane.

## Architektura WWW
Pola per wydanie: videoId (po sprawdzeniu publiczności), youtubeUrl, coverAsset, spotifyUrl, appleMusicUrl, youtubeMusicUrl, releaseDate, ISRC, UPC, persona (tylko po zatwierdzeniu), rightsStatus. Linków nieaktywowanych nie pokazywać. Dział streaming jest rozszerzeniem katalogu muzyki, a nie osobnym systemem.
