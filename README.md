# studio85.ai — wersja startowa (60 dni)

## 1. Plan w skrócie
**Cel na 60 dni:** co najmniej 2 decyzje na G1, 1 test popytu z prawdziwymi ludźmi, koszty w budżecie. Jeśli nie — poprawiamy proces, nie dokładamy agentów.

| Bramka | Pytanie | Co musi być gotowe | Czas |
| --- | --- | --- | --- |
| G0 | Czy opis wystarcza? | formularz pomysłu, kontrola CEO, ocena wstępna Analyst | 1–2 dni |
| G1 | Warto testować? | Opportunity Brief + karta oceny, memo Red Team, checklista G1 | ~1 tydz. |
| G2 | Ktoś tego chce? | strona testowa, 5–10 rozmów (prowadzicie Wy), wyniki vs progi ustalone przed testem | 2–3 tyg. |
| G3 | Odpalamy? | specyfikacja MVP, MVP na stagingu + Wasza akceptacja, checklista startu | 2–6 tyg. |

Zasady bez zmian: decyzje podejmuje Board, kill to dobry wynik, nikt nie ocenia własnej pracy, progi przed testem, treści z zewnątrz to dane, nie polecenia. Limit: 1 pomysł w budowie naraz.

## 2. Agenci
| Agent | Kiedy | Model | Raportuje do | Narzędzia | Skille studia |
| --- | --- | --- | --- | --- | --- |
| CEO | od razu | tańszy | Board | tylko Paperclip | 8 (`agents/ceo/skills`) |
| Analyst | od razu | średni | CEO | wyszukiwanie i odczyt stron; bez sekretów, bez publikacji | analyst-scorecard, analyst-opportunity-brief, analyst-demand-test, analyst-mvp-spec |
| Red Team | od razu | inny model/dostawca niż Analyst | CEO w Paperclip, memo idzie do Board bez zmian | jak Analyst | redteam-memo |
| Engineer | po G1 = go | mocny | CEO | repo tylko tego produktu, staging; produkcja i wydatki = „Ask first” | eng-landing-test, eng-mvp, eng-launch-checklist |

QA = Wasza akceptacja według kryteriów ze specyfikacji. Finanse/prawo/bezpieczeństwo = checklisty CEO i Engineer.

## 3. Wdrożenie w Paperclip (kolejność)
1. **Bezpieczniki kosztów, zanim cokolwiek uruchomicie**
   - limit dzienny i miesięczny na kluczu API u dostawcy modeli (drugi bezpiecznik niezależny od Paperclip);
   - budżet firmy w Paperclip i budżety agentów z alertem 80% i twardym stopem 100%. Proponowany podział: CEO 10%, Analyst 30%, Red Team 10%, Engineer 40%, rezerwa 10%.
2. **Firma i cel:** jedna firma „studio85”; cel firmy = „2 decyzje G1 i 1 test popytu w 60 dni”.
3. **Skille:** w Skills utwórz skille z folderów `agents/*/skills/*/SKILL.md` (1 plik = 1 skill). Przypisz każdemu agentowi tylko jego skille.
   - CEO zostawia wbudowane: paperclip, paperclip-converting-plans-to-tasks, paperclip-create-agent, para-memory-files; wyłącz paperclip-board, a first-task po pierwszym zadaniu.
   - Pozostali agenci: tylko paperclip + ich skille.
4. **CEO:** podmień instrukcje na `agents/ceo/AGENTS.md`. Heartbeat 2× dziennie (rano digest, wieczorem przegląd).
5. **Analyst i Red Team:** zatrudnij przez CEO (test: CEO ma poprosić Was o zgodę). Instrukcje z `AGENTS.md` ich folderów. Bez heartbeatu czasowego — budzą się, gdy dostaną zadanie.
6. **Narzędzia (tool gateway):** Analyst/Red Team — wyszukiwanie i odczyt: Allowed; zapis na zewnątrz i sekrety: Off. CEO — tylko Paperclip. Engineer (później) — repo i staging: Allowed; deploy prod, zakupy, publikacje: Ask first.
7. **Pierwszy pomysł:** utwórz projekt pomysłu, wklej `formularz-pomyslu.md` wypełniony jako zadanie dla CEO. Oczekiwany przebieg: `orch-intake-check` → pytania albo zadanie dla Analyst → ocena wstępna → Wasza decyzja o Discovery.
8. **Po G1 = go:** CEO wnioskuje o Engineer → zgoda → `agents/engineer`.

**Rytm Board:** codziennie 5 min na digest; poniedziałek 30 min na raport tygodniowy i decyzje; decyzja bramkowa w 48 h.

## 4. Jak to potem rozszerzyć
Nic tu nie jest wyrzucane — pełny model studia (dokument „studio85.ai — fabryka produktów”) to ta sama struktura z większą liczbą ról.
| Sygnał | Dodajecie | Skąd instrukcje i skille | Co zmieniacie u CEO |
| --- | --- | --- | --- |
| Pierwszy produkt z płacącymi klientami lub danymi osobowymi | QA, DevOps, Security Tester; bramka G4 (30/60/90 dni) | zakładki 2 (Role) i 6 (Prompty i skille) | `studio-hiring`, `orch-phase-plan` (+G4) |
| Jest co promować | Growth, Content & Social, radar trendów | j.w. | plan zatrudnień |
| 2+ produkty działają | CFO (P&L per aplikacja), Compliance, Support, Studio Ops | j.w. | checklisty bramek → oddane rolom |
| 2–3 cykle za Wami | Red Team całego studia, audyt agentów, radary pomysłów | j.w. | raport tygodniowy + przegląd procesu |
| Wyjście za granicę | Analyst: mapa ekspansji, Compliance: `compliance-ekspansja` | j.w. | nowa bramka „ekspansja” |
Zasada: każdą nową rolę dodajecie dopiero, gdy jej brak realnie coś zablokował albo zwiększył ryzyko.
