---
name: eng-launch-checklist
description: Użyj przed G3, żeby sprawdzić minimum bezpieczeństwa i gotowości produkcyjnej MVP.
---
# Checklista
- [ ] Brak sekretów w repo (skan), sekrety w menedżerze sekretów
- [ ] Skan zależności bez podatności krytycznych; wersje przypięte
- [ ] Logowanie i uprawnienia z gotowej usługi; użytkownik widzi tylko swoje dane
- [ ] Walidacja wejścia, ochrona przed typowymi atakami (OWASP Top 10), limity zapytań na formularzach
- [ ] HTTPS, nagłówki bezpieczeństwa
- [ ] Osobne środowiska i klucze dla staging i produkcji
- [ ] Logi bez danych osobowych i sekretów
- [ ] Kopia zapasowa bazy + jedno próbne odtworzenie
- [ ] Monitoring: czy strona działa, alert do Board
- [ ] Koszt miesięczny infrastruktury i usług
- [ ] Jeśli produkt używa AI wobec użytkownika: oznaczenie i ochrona przed prompt injection w danych użytkownika
# Wyjście
Tabela: punkt | OK / brak | działanie. Każdy „brak” = zadanie albo świadoma decyzja Board.
