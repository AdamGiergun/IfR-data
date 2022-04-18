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
    <li><a href="#o-mnie">O mnie</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

### O projekcie

Część projektu stworzonego jako szybka odpowiedź na ogromny kryzys humanitarny wywołany wojną na Ukrainie.<br>
Jest to repozytorium zawierające listę miejsc udzielających pomocy ukraińskim uchodźcom i wykorzystywane przez moją aplikację na Androida, [dostępna tutaj](https://play.google.com/store/apps/details?id=eu.adamgiergun.infoforukrainianrefugees).<br>
Miejsca mogą posiadać adresy, numery telefonów, e-maile, strony internetowe, informacje o świadczonych usługach, itp..

Ponieważ wprowadzenie tych danych dla jak największej liczby miejsc w możliwie najkrótszym czasie jest dla jednej osoby "mission impossible", to zdecydowanie potrzebuję pomocy.<br>
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
* Jeśli nie zaszkodzi to projektowi: udostępnić kod źródłowy w formie projektów "open source", dla zapewnienia pełnej transparentności (dane aplikacji są już udostępnione na warunkach [licencji GNU GPL](https://github.com/AdamGiergun/IfR-data/blob/main/LICENSE)).
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

<!-- ABOUT_ME -->

## O mnie

* Jestem specjalistą IT, w ostatnich latach głównie rozwijającym własne projekty aplikacji na system Android i samodoskonalącym się w sztuce programowania.
  
* Mam za sobą wieloletnie doświadczenie w branży IT, z czego większość to praca w małej, dynamicznej firmie high-tech, w której bardzo liczyło się kreatywne podejście do projektów. 
  Uczestniczyłem w niej w wielu projektach zespołowych. Często moja praca była ważną (a czasem kluczową) ich częścią, jak również prowadziłem wiele jednoosobowych projektów, za które odpowiadałem w całości.
  
* Z ostatnich lat mam też za sobą również doświadczenie z pracy w miedzynarodowym zespole rozproszonym w różnych lokalizacjach, dla firmy [DIO-soft](http://www.dio-soft.com/en/) z Ukrainy,
  zakontraktowanej przez globalną korporację finansową (niestety utraciła ona ten kontrakt przez obawy koncernu związane z agresją Rosji).
  
* Oprócz doświadczeń praktycznych, osiem lat temu ukończyłem studia na [Uniwersytecie Ekonomicznym w Krakowie](https://uek.krakow.pl/), 
  na kierunku [Informatyka Stosowana](https://studiuj.uek.krakow.pl/listings/kierunek-informatyka-stosowana-niestacjonarne-i-stopien/) [(specjalność Inżynieria Oprogramowania)](https://studiuj.uek.krakow.pl/listings/specjalnosc-inzynieria-oprogramowania-niestacjonarne-i-stopien/).
  Studia były opłacone z funduszy Unii Europejskiej (co wiązało się z podwyższonymi wymogami). W ich trakcie zdobywałem stypendium za wyniki w nauce i ukończyłem je z wynikiem "bardzo dobrym".  
  Oprócz zajęć dotyczących czysto matematyczno-informatycznej wiedzy, poznawałem tam też podstawy np. ekonomii, ekonomiki przedsiębiorstw, zarządzania, psychologii, czy prawa.

* Jak chodzi o projekty o znaczeniu społecznym, to obawiam się, że jestem "dziedzicznie uwarunkowany" w tym kierunku :wink: <br>
  Dwoje z moich dziadków było w swoim sąsiedztwie bardzo znanych z działań na rzecz lokalnej społeczności i w efekcie byli wybierani do Rady Miejskiej.<br>
  Oboje z moich rodziców otrzymali odznaki państwowe za swoją działaność społeczną.<br>
  W efekcie zawsze gdzieś w głębi mnie tkwiła chęć do tego, żebym spróbował przynajmniej dorównać ich osiągnięciom.<br>
  Ja sam przez lata udzielałem się w różny sposób w działaniach społecznościowych i tworzenie takiego projektu jak ten jest dla mnie o wiele ważniejsze niż zdobycie dobrze płatnej pracy jako programista.

* Jeśli miałbym opisać inne swoje zalety, istotne pod kątem zdolności do prowadzenia tego projektu, to byłyby to:
  Rozległa wiedza ogólna (nie tylko z zakresu IT).
  Kreatywność (moim "problemem" jest nadmiar, a nie brak pomysłów). :wink:
  Zdolność do szybkiego przyswajania sobie bardzo specjalistycznej wiedzy, połączona ze stosowaniem jej z powodzeniem w rozwiązaniach praktycznych.
  Zdolność do ciężkiej wytrwałej pracy, po to aby realizować ambitne cele.
  Komunikatywność i niekonfliktowa, otwarta osobowość.

<p align="right">(<a href="#top">powrót</a>)</p>
