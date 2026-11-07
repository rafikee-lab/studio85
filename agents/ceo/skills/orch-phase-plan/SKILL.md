---
name: orch-phase-plan
description: Użyj na starcie każdej fazy (Discovery, Walidacja, Budowa), żeby rozbić cel na małe zadania z właścicielami, budżetem i limitem przebiegów.
---
# Wejście
Decyzja Board z poprzedniej bramki (cel, budżet, termin) i artefakty z poprzedniej fazy.

# Artefakty wymagane na bramkach
| Bramka | Artefakty | Właściciel → reviewer |
| --- | --- | --- |
| G1 Warto testować? | Opportunity Brief z kartą oceny | Analyst → Red Team |
| | Red Team memo | Red Team → Board |
| | Checklista G1 | CEO (`studio-gate-checklists`) → Board |
| G2 Ktoś tego chce? | Plan testu popytu z progami (przed testem!) | Analyst → Red Team, zatwierdza Board |
| | Strona testowa | Engineer → Board (publikacja za zgodą Board) |
| | Wyniki testu + podsumowanie rozmów | Analyst → Red Team |
| G3 Odpalamy? | Specyfikacja MVP | Analyst → Engineer (wykonalność), zatwierdza Board |
| | MVP na stagingu + testy | Engineer → Board (akceptacja wg kryteriów) |
| | Checklista startu (bezpieczeństwo, prawo, koszty) | Engineer + CEO → Board |

# Kroki
1. Dla każdego artefaktu 1–3 zadania. Każde: właściciel, reviewer (inna rola), definicja „done”, projekt pomysłu, termin, limit 3 przebiegów, limit budżetu.
2. Kolejność i zależności; równolegle maksymalnie 3 agentów.
3. Budżet fazy rozpisany na zadania, 15% rezerwy.

# Wyjście
Zadania w Paperclip + plan fazy w zadaniu nadrzędnym (cel, artefakty, kolejność, budżet, termin bramki).

# Zasady
Zadanie na więcej niż 2 przebiegi — dziel. Nie twórz zadań dla nieistniejących ról.
