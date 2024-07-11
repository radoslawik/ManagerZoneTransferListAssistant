# ManagerZoneTransferListAssistant

Improve your transfer list experience and enjoy new features

### Opis
Projekt składałby się z 2 części, serwera z bazą danych oraz aplikacji desktopowej dla użytkowników. Część serwerowa co jakiś czas (1-2 razy w ciągu dnia) skanowałaby listę transferową i zapisywała informacje o wystawionych zawodnikach do bazy danych. Aplikacji z kolei prosiłaby serwer o dane i prezentowała użytkownikom.


### Ficzery
 - Logowanie. Użytkownicy mogą zalogować się do swojego konta (można użyć po prostu cookie z przeglądarki albo login + hasło) aby zyskać dostęp do większej ilości funkcji.
 - Caching. Żeby nie pobierać danych z serwera co chwilę można zapisywać je na dysku i odświeżać tylko jeśli na serwerze pojawią się nowe dane. Jeśli użytkownik jest zalogowany to można pobierać informacje z listy transferowej bezpośrednio z aplikacji i zapisywać w cachu. Oczywiście trzeba wszędzie dodać timestamps'y, żeby wiedzieć które informacje są nowe, a które stare.
 - Formuły. Użytkownicy mogą definiować swoje formuły obliczające jakość zawodnika dla dalej pozycji (takie jak np. na mzlive, oxy.se, można je nawet dodać jako default)
 - Filtrowanie listy. Nowe filtry takie jak HP, LP, bloki na umiejętnościach, wyniki formuł i kto wie co jeszcze :)
 - Sortowanie listy. Nowe metody sortowania takie jak trending (zawodnicy, którzy są licytowani przez kilku graczy) i offers (zawodnicy, których cena znacząco spadła od ostatniego wystawienia na rynek)
 - Widok zawodnika. Dodanie do widoku zawodnika informacji o jego ostatnich transferach, porównanie cen z zawodnikami o podobnych umiejętnościach (tutaj trzeba by było wymyślić jakiś algorytm), wyniki formuł, opcje pokazania najlepszej i najgorszej wersji wytrenowania
 - Obserwowanie zawodników. Możliwość edycji swojej listy obserwowanych z poziomu aplikacji (tylko dla zalogowanych)
 - Porównanie zawodników. Możliwość porównywania zawodników z listy transferowej oraz zawodników z drużyny (tylko dla zalogowanych). Piłki na umiejętnościach, wyniki z formuł, etc.
 - Bidowanie zawodników (nice to have). Możliwość ustawienia automatycznego licytowania zawodnika do ustawionego górnego limitu (tylko dla zalogowanych). Może być z tym ciężko, bo wtedy aplikacja musiałaby działać w tle. Inna opcja to użycie serwera, ale wtedy wszyscy mieliby takie samo IP i pewnie spowodowałoby to upadek listy transferowej i całego mzeta :D
 - User experience. Przyjazny i intuicyjny interfejs graficzny, optymalizacja wszystkiego co się da, np. kiedy użytkownik przegląda listę transferową w aplikacji nowe dane mogą być pobierane tylko dla tych zawodników, którzy są aktualnie przeglądani. Możliwość wyłączenia tej funkcji i dodania ikonki refresh, jeśli użytkownik woli oglądać stare dane, ale mieć lepszy performance.
