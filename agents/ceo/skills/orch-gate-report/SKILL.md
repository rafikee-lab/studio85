---
name: orch-gate-report
description: Użyj na końcu każdej fazy, żeby zebrać artefakty, sprawdzić ich kompletność i przygotować Board Raport bramki z rekomendacją.
---
# Cel
Board podejmuje decyzję na podstawie jednego, kompletnego raportu.

# Kroki
1. Sprawdź, czy wszystkie artefakty fazy są gotowe i przeszły review. Brakujący artefakt = raport nie idzie do Board.
2. Porównaj wyniki z progami ustalonymi przed fazą (nie po).
3. Stanowisko Red Team cytuj bez łagodzenia.
4. Policz zużyty budżet względem planu.
5. Sformułuj rekomendację: go / kill / pivot, z jednym zdaniem uzasadnienia.

# Wyjście (szablon)
```
# Bramka <G1–G3>: <nazwa>
Co zatwierdzamy: <1 zdanie>
Największe ryzyko: <1 zdanie>
Co się stanie przy odmowie: <1 zdanie>
Termin decyzji: <data>

- Rekomendacja CEO: go / kill / pivot — <uzasadnienie>
- Wynik względem progów: <próg → wynik>
- Karta oceny: wstępna <X>/90 → obecna <Y>/90 (pewność W/S/Z)
- Najważniejsze ryzyka i stanowisko Red Team:
- Zużyty budżet vs plan:
- Wniosek o budżet na kolejną fazę:
- Artefakty (linki):
- Decyzja Board i data: <wypełnia Board>
```

# Zasady
Nie zmieniasz progów po fakcie i nie ukrywasz słabych wyników. Rekomendujesz; nie decydujesz.
