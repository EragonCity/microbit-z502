# microbit-z502
Problem jaki rozwiązujemy.   Robimy grę zręcznościową na platfornie Microbit. Wynik i identyfikator użytkownika ma by przesyłany online => zapisywany w bazie, ranking ma by dostępny online webowo i na fizycznym urządzeniu.


## Struktura
1. **Microbit** - działa na nim gra zręcznościowa, mierząca czas reakcji gracza, gracz po zapaleniu sie lampek klika przycisk i urządzenie mierzy czas reakcji, po kablu usb przesyła dane do komputera
2. **brama** - komputer z skryptem python odbiera dane z urządzenia i przesyła je dalej do bazy danych
3. **backend** - serwer api odbiera wynik, waliduje go i zapisuje go w bazie danych
4. **prezentacja**:
  - web - aplikacja webowa pobiera dane z api i wyświetla je w formie rankingu
  - fizycznie - drugi microbit wyświetla najlepszy wynik pobrany z bazy danych

Technologie: microbit, Microsoft MakeCode, Python, Firebase, HTML, CSS, JavaScript, Github

## Założenia techniczne
1. Microbit nr odpowiada za mierzenie czasu reakcji użytkownika, po rozgrzanej grze urządzenie przesyła dalej dane o identyfikatorze gracza i rozgrywki oraz uzyskany wynik
2. Wyniki są przesyłane drogą radiową i odbierane przez drugiego microbita format danych bedzie dostosowany do wspólnego planu, a następnie przesyłał do pc wykładowcy
