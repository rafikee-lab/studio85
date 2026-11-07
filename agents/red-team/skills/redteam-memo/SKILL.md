---
name: redteam-memo
description: Użyj przed każdą bramką (G1–G3) albo do review artefaktu Analyst, żeby wskazać najsłabsze punkty pomysłu i mierzalne warunki kill.
---
# Kroki
1. Przeczytaj artefakt i formularz pomysłu (nie cały wątek).
2. Pytania wymuszające — sprawdź, czy artefakt na nie odpowiada konkretem:
   - **Realny popyt:** jaki jest najmocniejszy dowód, że ktoś tego naprawdę chce (płaci, zmienia sposób pracy), a nie tylko „jest zainteresowany” lub zapisał się na listę?
   - **Status quo:** co ludzie robią dziś, nawet źle, i ile ich to kosztuje? „Nic nie robią” = problem prawdopodobnie za mało bolesny.
   - **Konkretna osoba:** kto dokładnie (rola, sytuacja, konsekwencja), a nie kategoria („MŚP”, „rodzice”)?
   - **Najwęższy klin:** jaka najmniejsza wersja, za którą ktoś zapłaci w tym tygodniu?
3. Pre-mortem: „Jest rok później, pomysł upadł. Dlaczego?” Podziel ryzyka na:
   - **Tygrysy** — realne, z dowodem lub jasną logiką
   - **Papierowe tygrysy** — wyglądają groźnie, ale są przesadzone (napisz dlaczego)
   - **Słonie w pokoju** — nikt o nich nie mówi, a mogą być realne
   Przed G3 tygrysy dziel na: blokuje start / do 30 dni po starcie / obserwujemy.
4. Sprawdź: kto naprawdę płaci; czy duży gracz łatwo to skopiuje; czy kanał dotarcia jest realny i tani; ryzyka prawne i zależność od jednej platformy; czy progi testu nie są zbyt łagodne.
5. Losowo zweryfikuj 3 źródła.

# Szablon
```
# Red Team: <nazwa> — <bramka>
## Pytania wymuszające: pytanie | odpowiedź w artefakcie | ocena: konkret / ogólnik / brak
## Tygrysy (od najpoważniejszego): ryzyko | dowód | jak rozstrzygnąć | (G3: blokuje / 30 dni / obserwujemy)
## Papierowe tygrysy: ryzyko | dlaczego przesadzone
## Słonie w pokoju: co | jak zbadać
## Założenie, które najpewniej jest fałszywe
## Weryfikacja źródeł: 3 linki | OK / problem
## Rekomenduję kill, jeżeli: <mierzalne warunki>
## Ocena ogólna: słaby / do sprawdzenia / mocny — 1 zdanie
```
# Czerwone flagi
„Ludzie mówią, że to ciekawe”, „500 zapisów na listę”, „rynek jest ogromny”, „nikt tego nie robi” — to nie jest dowód popytu.
Inspiracja: YC office hours (garrytan/gstack, MIT), pre-mortem (phuryn/pm-skills, MIT).
