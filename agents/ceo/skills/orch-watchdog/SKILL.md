---
name: orch-watchdog
description: Użyj przy każdym przeglądzie pracy (heartbeat), żeby wyłapać blokery, pętle, zadania bez postępu i przekroczenia budżetu, zanim spalą tokeny.
---
# Co sprawdzasz
1. **Budżet:** zadania, agenci, projekty i faza ≥ 80% budżetu → wstrzymaj nowe prace w tym zakresie i zgłoś Board.
2. **Pętle:** zadanie z ≥ 3 przebiegami bez nowego artefaktu albo z powtarzanymi krokami → stop, krótka diagnoza, eskalacja.
3. **Zastój:** zadanie bez postępu > 48 h → zapytaj właściciela o bloker; jeśli to zależność — przestaw kolejność; jeśli brak decyzji — wniosek do Board.
4. **Odmowy i „nie wiem”:** doprecyzuj zadanie albo przekaż innemu agentowi lub modelowi; po drugiej próbie eskalacja. Zapisz przypadek.
5. **Równoległość:** maksymalnie 3 agentów pracujących naraz; nadmiarowe zadania czekają w kolejce.
6. **Porządek kosztów:** zadania bez projektu aplikacji — przypnij albo uzasadnij jako koszt wspólny.

# Wyjście
Krótka lista działań (co zatrzymano, co przekazano, co eskalowano) dopisywana do codziennego digestu.

# Zasady
Lepiej zatrzymać i zapytać niż pozwolić agentowi próbować dalej. Każda kolejna próba kosztuje.
