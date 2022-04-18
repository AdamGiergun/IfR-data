<h1 align="center">Repozytorium danych dla androidowej aplikacji<br>"IfR - Informacje dla uchodzców"</h1>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Spis treści</summary>
  <ol>
    <li><a href="#o-projekcie">O projekcie</a></li>
    <li><a href="#cele">Cele</a></li>
    <li><a href="#stworzony-przy-pomocy">Stworzony przy pomocy</a></li>
    <li><a href="#jak-można-wesprzeć-ten-projekt">Jak można wesprzeć ten projekt</a>
    <ol>
    <li><a href="#tłumaczenia">&nbsp;&nbsp;&nbsp;&nbsp;Tłumaczenia</a></li>
    <li><a href="#dane">Dane</a></li>
    <li><a href="#spot">&nbsp;&nbsp;&nbsp;&nbsp;Spot</a></li>
    <li><a href="#territorial-unit">&nbsp;&nbsp;&nbsp;&nbsp;Territorial unit</a></li>
    <li><a href="#service">&nbsp;&nbsp;&nbsp;&nbsp;Service</a></li>
    </ol></li>
    <li><a href="#podziękowania">Podziękowania</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

### O projekcie

Część projektu stworzonego jako szybka odpowiedź na ogromny kryzys humanitarny wywołany wojną na Ukrainie.<br>
Jest to repozytorium zawierające listę miejsc udzielających pomocy ukraińskim uchodźcom i wykorzystywane przez moją aplikację na Androida, [dostępna tutaj](https://play.google.com/store/apps/details?id=eu.adamgiergun.infoforukrainianrefugees).<br>
Miejsca mogą posiadać adresy, numery telefonów, e-maile, strony internetowe, informacje o świadczonych usługach, itp..

Ponieważ wprowadzenie tych danych dla jak największej liczby miejsc w krótkim czasie jest dla jednej osoby "mission impossible", to zdecydowanie potrzebuję pomocy.<br>
Poniżej znajdują się instrukcje dotyczące przygotowywania tych danych.

### Cele

Teraz:
* Zaimplementowanie zaawansowanych możliwości odbierania wiadomości (bardzo ograniczone są już obecne). Wiadomości to byłyby: ważne komunikaty, informacje o wydarzeniach, itp.<br>
  Wiadomości byłyby adresowane dla konkretnej jednostki terytorialnej i posiadałyby określony zakres czasowy ważności.<br>
  Użytkownicy mieliby możliwość wyboru jednostek terytorialnych, dla których chcieliby otrzymywać wiadomości.<br>

Krótkoterminowe:
* Stworzyć listę (przynajmniej) większości miejsc udzielających pomocy uchodźcom.
* Zapewnić wysokiej jakości tłumaczenia.<br>
  [Daj mi znać](mailto:adam.giergun@gmail.com), jeśli chcesz mi pomóc w tym zadaniu.<br>
  Proszę, zacznij w takim wypadku tytuł e-maila od `#IfR-helpOffer: `.

Dłuższoterminowe:
* Stworzenie organizacji prowadzącej ten projekt i zatrudniającej osoby niezbędne do jego rozwoju i utrzymania. 
* Stworzenie narzędzi do wprowadzania danych do bazy (np. wygodny interfejs dla przeglądarki internetowej), oraz API umożliwiające dostęp do tych danych przez interfejsy użytkownika (strona internetowa, aplikacje, wtyczki).
* Stworzenie interfejsów użytkownika dla innych platform (strona internetowa, aplikacje na inne systemy).
* Stworzenie wtyczki do stron internetowych, aby umożliwić każdemu chętnemu udostępnienie wybranego zakresu danych z bazy projektu na swojej stronie internetowej.

Długoterminowe:
* Niestety ten kryzys uchodźczy nie jest jedynym. Mam nadzieję przekształcić ten projekt w coś stałego, by mógł służyć pomocą w każdym kryzysie humanitarnym.<br>
  Zachęcam do kontaktu, jeśli chcesz mi w tym pomóc: [mój e-mail to](mailto:adam.giergun@gmail.com) - proszę, pamiętaj w takim wypadku o rozpoczęciu tytułu e-maila od `#IfR-permanent: `.
<p align="right">(<a href="#top">powrót</a>)</p>

### Stworzony przy pomocy

* [Android Studio](https://developer.android.com/studio)

<p align="right">(<a href="#top">powrót</a>)</p>

<!-- CONTRIBUTION -->

### Jak można wesprzeć ten projekt

Najpilniejsze byłoby dostarczenie mi jak najlepszej jakości [tłumaczeń](https://github.com/AdamGiergun/IfR-data#translations) oraz danych dla aplikacji.
Najlepiej aby dane przygotowane były w formacie JSON, zgodnie z proponowanym przeze mnie standardem. Wiecej szczegółów poniżej: [Dane](https://github.com/AdamGiergun/IfR-data#dane)<br>
Używanie Android Studio do wprowadzania tych danych nie jest koniecznością, więc spójrz na [informacje o alternatywach](https://github.com/AdamGiergun/IfR-data/issues/1)

### &nbsp;&nbsp;&nbsp;&nbsp;Tłumaczenia
* Wysoce potrzebne są bardzo dobrej jakości tłumaczenia dla wszystkich plików README w tym repozytorium, a także dla [strings](https://github.com/AdamGiergun/IfR-data/blob/main/data/strings.xml) używanych w aplikacji.

### Dane
Dane są podzielone na trzy typy: [spot](https://github.com/AdamGiergun/IfR-data#spot), [territorial unit](https://github.com/AdamGiergun/IfR-data#territorial-unit) i [service](https://github.com/AdamGiergun/IfR-data#service).

### &nbsp;&nbsp;&nbsp;&nbsp;Spot
* `Spot` zawiera wszystkie informacje o miejscu.<br>
  Plik danych `spotów` można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json).<br>
  Instrukcje można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/), wybierając konkretny plik `README_SPOT_<akronim języka>.md`.

### &nbsp;&nbsp;&nbsp;&nbsp;Territorial unit
* `Territorial Unit`, czyli jednostka terytorialna to jedna z właściwości miejsca, wywodząca się z podziału administracyjnego danego kraju.<br>
  Dla Polski przeszukiwalny wykaz jednostek terytorialnych wraz z identyfikatorami jest dostarczany przez Główny Urząd Statystyczny i można go znaleźć [tutaj](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default). <br>
  Ponieważ identyfikatory pochodzą ze standardu opartego na ISO 19000, podejrzewam, że inne kraje muszą używać równoważnych list.<br>
  Jeśli wiesz, gdzie znaleźć takie listy [daj mi znać](https://github.com/AdamGiergun/IfR-data/issues/2). <br>
  Plik danych jednostek terytorialnych można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json). <br>
  Instrukcje można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/), wybierając konkretny plik `README_TU_<akronim języka>.md`.

###  &nbsp;&nbsp;&nbsp;&nbsp;Service
* `Service` to usługa oferowana przez dany `spot`.<br>
  Plik danych usług można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json). <br>
  Instrukcje można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/), wybierając konkretny plik `README_SERVICE_<akronim języka>.md`.

<p align="right">(<a href="#top">powrót</a>)</p>

<!-- ACKNOWLEDGMENTS -->

## Podziękowania

* To miejsce czeka na `Ciebie` :smile:

<p align="right">(<a href="#top">powrót</a>)</p>
