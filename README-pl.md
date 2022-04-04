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

Część projektu stworzonego, jako szybka odpowiedź na ogromny kryzys humanitarny wywołany wojną na Ukrainie.<br>
Jest to repozytorium zawierające listę miejsc udzielających pomocy ukraińskim uchodźcom i wykorzystywane przez moją aplikację na Androida, [dostępna tutaj](https://play.google.com/store/apps/details?id=eu.adamgiergun.infoforukrainianrefugees).<br>
Miejsca mogą posiadać adresy, numery telefonów, e-maile, strony internetowe, informacje o świadczonych usługach, itp..

Ponieważ wprowadzenie tych danych dla jak największej liczby miejsc w krótkim czasie jest dla jednej osoby "mission impossible", to zdecydowanie potrzebuję pomocy.<br>
Poniżej znajdują się instrukcje dotyczące przygotowywania tych danych.

### Cele

Teraz:
* Dodać możliwość zgłaszania nowych miejsc bezpośrednio w aplikacji

Krótkoterminowe:
* Stworzyć listę (przynajmniej) większości miejsc udzielających pomocy uchodźcom.
* Zapewnić dobre tłumaczenia.<br>
  [Daj mi znać](mailto:adam.giergun@gmail.com), jeśli chcesz mi pomóc w tym zadaniu.<br>
  Proszę, zacznij w takim wypadku tytuł e-maila od `#IfR-data: `.

Dłuższoterminowe:
* Stworzyć narzędzia do wprowadzania danych do bazy (np. jakiś wygodny interfejs przeglądarkowy).
* Utwórz interfejs użytkownika dla innych platform.

Długoterminowe:
* Niestety ten kryzys uchodźczy nie jest jedynym. Mam nadzieję przekształcić ten projekt w stały, by mógł służyć pomocą w każdym podobnym kryzysie. Zapraszam do kontaktu, jeśli chcesz mi w tym pomóc: [mój e-mail to](mailto:adam.giergun@gmail.com) - pamiętaj wtedy o `#IfR-permanent: `w temacie e-maila.
<p align="right">(<a href="#top">powrót</a>)</p>

### Stworzony przy pomocy

* [Android Studio](https://developer.android.com/studio)

<p align="right">(<a href="#top">powrót</a>)</p>

<!-- CONTRIBUTION -->

### Jak można wesprzeć ten projekt

Najlepszym sposobem na wsparcie tego projektu będzie dostarczenie mi [tłumaczeń](https://github.com/AdamGiergun/IfR-data#translations) oraz danych aplikacji w formacie JSON, wprowadzonych zgodnie z proponowanym przeze mnie standardem.<br>
Używanie Android Studio do wprowadzania danych nie jest koniecznością, więc spójrz na [informacje o alternatywach](https://github.com/AdamGiergun/IfR-data/issues/1)

### &nbsp;&nbsp;&nbsp;&nbsp;Tłumaczenia
* Potrzebne są dobre tłumaczenia dla wszystkich plików README w tym repozytorium, a także dla [strings](https://github.com/AdamGiergun/IfR-data/blob/main/data/strings.xml) używanych w aplikacji.

### Dane
Dane są podzielone na trzy rodzaje: [spot](https://github.com/AdamGiergun/IfR-data#spot), [territorial unit](https://github.com/AdamGiergun/IfR-data#territorial-unit) i [service](https://github.com/AdamGiergun/IfR-data#service).

### &nbsp;&nbsp;&nbsp;&nbsp;Spot
* `Spot` zawiera wszystkie informacje o miejscu.<br>
  Plik danych spotów można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json).<br>
  Instrukcje można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/), wybierając konkretny plik README_SPOT_<akronim języka>.md

### &nbsp;&nbsp;&nbsp;&nbsp;Territorial unit
* `Territorial Unit`, czyli jednostka terytorialna to jedna z właściwości miejsca, wywodząca się z podziału administracyjnego kraju.<br>
  Dla Polski przeszukiwalny wykaz jednostek terytorialnych wraz z identyfikatorami jest dostarczany przez Główny Urząd Statystyczny i można go znaleźć [tutaj](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default).<br>
  Ponieważ identyfikatory pochodzą ze standardu opartego na ISO 19000, podejrzewam, że inne kraje posiadają równoważne listy.<br>
  Jeśli wiesz, gdzie znaleźć takie listy [daj mi znać](https://github.com/AdamGiergun/IfR-data/issues/2). <br>
  Plik danych jednostek terytorialnych można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json). <br>
  Instrukcje można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/), wybierając konkretny plik README_TU_<akronim języka>.md.

###  &nbsp;&nbsp;&nbsp;&nbsp;Service
* `Service` is (just as it name suggests) a service offered by the spot.
  Plik danych usług można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json).
  Instrukcje można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/), wybierając konkretny plik README_SERVICE_<akronim języka>.md.

<p align="right">(<a href="#top">powrót</a>)</p>

<!-- ACKNOWLEDGMENTS -->

## Podziękowania

* To miejsce czeka na Ciebie :smile:

<p align="right">(<a href="#top">powrót</a>)</p>
