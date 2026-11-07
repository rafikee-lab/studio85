---
name: eng-mvp
description: Użyj po G2 = go, żeby zbudować MVP według zatwierdzonej specyfikacji — historyjka po historyjce, z testami, na stagingu.
---
# Kroki
1. Przeczytaj specyfikację; niejasności i ryzyka wykonalności zgłoś CEO, zanim zaczniesz.
2. Plan: lista historyjek w kolejności, szacunek każdej, potrzebne usługi zewnętrzne (z kosztem).
3. Dla każdej historyjki: najpierw test dla kryterium akceptacji (Given/When/Then), zobacz, że nie przechodzi, potem kod, aż przejdzie.
4. Po każdej historyjce: uruchom pełne testy, deploy na staging, krótki komentarz w zadaniu (co działa, jak sprawdzić, wynik testów).
5. Na końcu: raport — kryteria spełnione X/Y, znane braki, koszt miesięczny utrzymania, instrukcja dla Board do akceptacji.

# Dowód przed deklaracją
Nie piszesz „działa”, „gotowe”, „naprawione”, dopóki w tym samym przebiegu nie uruchomisz komendy, która to dowodzi, i nie przeczytasz wyniku. W komentarzu podajesz dowód (np. „testy: 24/24, 0 błędów”). Słowa „powinno”, „chyba”, „raczej” = jeszcze nie sprawdzone.

# Błędy
Najpierw przyczyna, potem poprawka: odtwórz błąd, znajdź źródło, napraw, dodaj test, który go łapie. Po 3 nieudanych poprawkach — stop i komentarz do CEO.

# Zasady
Nic poza specyfikacją. Każda nowa zależność uzasadniona. Dane testowe, nigdy prawdziwe.
Inspiracja: verification-before-completion, systematic-debugging, test-driven-development (obra/superpowers, MIT).
