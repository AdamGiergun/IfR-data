<h1 align="center">Data repository for "IfR - Info for Refugees"<br>- an Android app</h1>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#objectives">Objectives</a></li>
    <li><a href="#built-with">Built With</a></li>
    <li><a href="#contribution">Contribution</a>
    <ol>
    <li><a href="#translations">&nbsp;&nbsp;&nbsp;&nbsp;Translations</a></li>
    <li><a href="#spot">&nbsp;&nbsp;&nbsp;&nbsp;Spot</a></li>
    <li><a href="#territorial-unit">&nbsp;&nbsp;&nbsp;&nbsp;Territorial unit</a></li>
    <li><a href="#service">&nbsp;&nbsp;&nbsp;&nbsp;Service</a></li>
    </ol></li>
    <li><a href="#credits">Credits</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

### About The Project

Part of a project created as a quick response to a huge humanitarian crisis caused by the War on Ukraine.<br>
It is repository containing list of spots providing help to Ukrainian refugees and used by my Android app, [available here](https://play.google.com/store/apps/details?id=eu.adamgiergun.infoforukrainianrefugees).<br>
Spots can have physical addresses, phone numbers, e-mails, websites, info about services provided, etc..

As entering this data for as many as possible spots in a short time is "mission impossible" for one person I obviously need a help.<br>
Below are instructions for preparing this data.

### Objectives

Short term:
* Create a list of (at least) most of the spots providing help for refugees.<br>
* Provide better translations: [let me know](mailto:adam.giergun@gmail.com) if you wanna help me with this task (please, start then e-mail subject with `#IfR-data: `).

Longer term:
* Create tools for entering data to the database (like a some feasible web interface).
* Create user interface for other platforms.

Much longer term:
* Unfortunately this refugee crisis is not the only one. I hope to convert this project into permanent, to serve in any similar crisis. Please feel free to contact me if you want to help me achieve it: [my e-mail](mailto:adam.giergun@gmail.com) with `#IfR-permanent: `in e-mail subject.

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

* [Android Studio](https://developer.android.com/studio)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTRIBUTION -->

### Contribution

The best way of supporting this project will be providing me with [translations](https://github.com/AdamGiergun/IfR-data#translations), and an app's data formatted as a JSON file, accordingly to the standard I propose.<br>
Using Android Studio for entering data is not a must, so look at the [info about alternatives](https://github.com/AdamGiergun/IfR-data/issues/1)

### &nbsp;&nbsp;&nbsp;&nbsp;Translations
* Good translations are needed for all READMEs in this repository, and also for [strings](https://github.com/AdamGiergun/IfR-data/blob/main/data/strings.xml) used in the app.

Data are structured in three types: [spot](https://github.com/AdamGiergun/IfR-data#spot), [territorial unit](https://github.com/AdamGiergun/IfR-data#territorial-unit) and [service](https://github.com/AdamGiergun/IfR-data#service).

### &nbsp;&nbsp;&nbsp;&nbsp;Spot
* `Spot` contains all the info about place.
  Spots data file can be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json).<br>
  For instructions look [here](https://github.com/AdamGiergun/IfR-data/tree/main/instructions), and find a proper `README_SPOT_<language acronym>.md`.
  
### &nbsp;&nbsp;&nbsp;&nbsp;Territorial unit
* `Territorial unit` is one of the properties of spot coming from administrative division of country.<br>
  For Poland searchable list of territorial units with ids is provided by Central Statistical Office, and can be found [here](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default),
  but as ids come from standard based on ISO 19000 I strongly suspect that other countries have equivalent lists.<br>
  If you know where to find such lists [let me know](https://github.com/AdamGiergun/IfR-data/issues/2). <br>
  Data file for territorial units is [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json). <br>
  For instructions look [here](https://github.com/AdamGiergun/IfR-data/tree/main/instructions), and find a proper `README_TU_<language acronym>.md`.

###  &nbsp;&nbsp;&nbsp;&nbsp;Service  
* `Service` is (just as it name suggests) a service offered by the spot.<br>
  Services data file can be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json). <br>
  For instructions look [here](https://github.com/AdamGiergun/IfR-data/tree/main/instructions), and find a proper `README_SERVICE_<language acronym>.md`.
  
<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->

## Credits

* This is a place waiting for `You` :smile:

<p align="right">(<a href="#top">back to top</a>)</p>
