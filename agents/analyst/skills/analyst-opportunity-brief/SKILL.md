---
name: analyst-opportunity-brief
description: Użyj w Discovery, żeby przygotować Opportunity Brief do bramki G1 „Warto testować?”.
---
# Szablon (maks. 2 strony)
```
# Opportunity Brief: <nazwa>
## 3 kluczowe wnioski (bez werdyktu go/kill)
## Problem i klient: konkretna osoba (rola, sytuacja), jak często, ile kosztuje ją problem dziś
## Jak radzą sobie dziś: obecne obejście i jego koszt (czas, pieniądze)
## Rynek: wielkość (przedział + metoda liczenia + źródła)
## Konkurencja: nazwa | link | cena | mocne | słabe | luka
## Kanały dotarcia: top 3 do testu, szacowany koszt pozyskania
## Ekonomia (uproszczona): cena, koszt obsługi klienta/mies., marża, wariant pesymistyczny
## Nazwa i domena: 3 propozycje z wolną domeną .pl/.com, brak oczywistego konfliktu ze znakiem towarowym (HIPOTEZA, jeśli nie sprawdzono w bazie)
## Ryzykowne założenia: założenie | kategoria | pewność W/S/Z | wpływ N/Ś/W | jak sprawdzić
## Hipotezy do testu popytu (z założeń o wysokim wpływie i niskiej pewności): hipoteza | metoda | próg sukcesu | próg kill
## Karta oceny: wynik końcowy vs wstępny
## Źródła
```
# Ryzykowne założenia — 8 kategorii
Przejrzyj każdą: **Wartość** (czy rozwiązuje problem, czy wrócą), **Użyteczność** (czy zrozumieją bez pomocy), **Opłacalność** (czy zapłacą, czy obsługa się spina, zgodność z prawem), **Wykonalność** (czy zbudujemy szybko i tanio), **Etyka** (czy może komuś zaszkodzić), **Dotarcie** (czy mamy kanał i komunikat), **Strategia** (czy łatwo skopiować, czy duży gracz wejdzie), **Zespół** (czy mamy wiedzę i czas).
Priorytet: wysoki wpływ + niska pewność → test popytu; wysoki wpływ + wysoka pewność → przyjmij; niski wpływ + wysokie ryzyko → powód do kill; reszta → odłóż.

# Zasady
Dowody przeciw pomysłowi równie widoczne jak za. Brief idzie do Red Team przed Board.
Inspiracja: identify-assumptions-new, prioritize-assumptions (phuryn/pm-skills, MIT).
