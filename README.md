<h1 align="center">Data repository for "IfR - Info for Refugees" Android app</h1>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-the-project">About The Project</a></li>
    <li><a href="#objectives">Objectives</a></li>
    <li><a href="#built-with">Built With</a></li>
    <li><a href="#contribution">Contribution</a>
    <ol><li><a href="#spot">Spot</a></li>
    <li><a href="#territorial-unit">Territorial unit</a></li>
    <li><a href="#service">Service</a></li></ol></li>
    <li><a href="#credits">Credits</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

### About The Project

Part of a project created as a quick response to a huge humanitarian crisis caused by the War on Ukraine.
It is repository containing list of spots providing help to Ukrainian refugees and used by my Android app, [available here](https://play.google.com/store/apps/details?id=eu.adamgiergun.infoforukrainianrefugees). 
Spots can have physical addresses, phone numbers, e-mails, websites, info about services provided, etc..

 As filling this data for as many as possible spots in a short time is "mission impossible" for one person I need help.
Below are instructions for entering this data.

### Objectives

Short term:
* Create a list of (at least) most of the spots providing help for refugees.
* Provide better translations ([let me know](mailto:adam.giergun@gmail.com) (please, start e-mail subject with #IfR-data: ) if you are willing to do it)

Long term: 
* Create tools for entering data to the database (like a some nice web interface).

<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

* [Android Studio](https://developer.android.com/studio)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTRIBUTION -->

### Contribution

The best way of supporting this project will be providing me with a data formatted as a JSON file, accordingly to the standard I set.
Using Android Studio for entering data is not a must, so look at the [info about alternatives](https://github.com/AdamGiergun/IfR-data/issues/1)

Data are structured in three types: "spot", "territorial unit" and "services".

### &nbsp;&nbsp;&nbsp;&nbsp; Spot
* Spot contains all the info about place.
  Spots data file can be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json)
  For instructions look [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/), and find a proper README_SPOT_(language).md
  
### &nbsp;&nbsp;&nbsp;&nbsp; Territorial unit
* Territorial unit is one of the properties of spot coming from administrative division of country.
  For Poland searchable list of territorial units can be found [here](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default),
  but as it is a standard based on ISO 19000 I strongly suspect that other countries have equivalent lists. 
  If you know where to find such lists [let me know](https://github.com/AdamGiergun/IfR-data/issues/2)
  Data file for territorial units is [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json)
  For instructions look [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/), and find a proper README_TU_(language).md

### &nbsp;&nbsp;&nbsp;&nbsp; Service  
* Service is (just as it name suggests) a service offered by the spot.
  Services data file can be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json)
  For instructions look [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/), and find a proper README_SERVICE_(language).md
  
<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->

## Credits

* This is a place waiting for You :smile:

<p align="right">(<a href="#top">back to top</a>)</p>
