<h1 align="center">Data repository for "IfR - Info for Refugees"<br>- an Android app</h1>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#Other-language-versions">Other language versions</a></li>
    <li><a href="#about-the-project">About the project</a></li>
    <li><a href="#objectives">Objectives</a></li>
    <li><a href="#built-with">Built with</a></li>
    <li><a href="#contribution">Contribution</a>
    <ol>
    <li><a href="#translations">&nbsp;&nbsp;&nbsp;&nbsp;Translations</a></li>
    <li><a href="#spot">&nbsp;&nbsp;&nbsp;&nbsp;Spot</a></li>
    <li><a href="#territorial-unit">&nbsp;&nbsp;&nbsp;&nbsp;Territorial unit</a></li>
    <li><a href="#service">&nbsp;&nbsp;&nbsp;&nbsp;Service</a></li>
    </ol></li>
    <li><a href="#credits">Credits</a></li>
    <li><a href="#about-me">About me</a></li>
  </ol>
</details>

<!-- OTHER LANGUAGE VERSIONS -->

### Other language versions

 * [Wersja polska](https://github.com/AdamGiergun/IfR-data/blob/main/README-pl.md)
 * [Українська версія (не готова)](https://github.com/AdamGiergun/IfR-data/blob/main/README-uk.md)
 * [Русская версия (не готова)](https://github.com/AdamGiergun/IfR-data/blob/main/README-ru.md)

<!-- ABOUT THE PROJECT -->

### About The Project

Part of a project created as a quick response to the huge humanitarian crisis caused by the war in Ukraine.<br>
It is a repository containing a list of spots providing assistance to Ukrainian refugees and used by my Android application, [available here](https://play.google.com/store/apps/details?id=eu.adamgiergun.infoforukrainianrefugees). <br>
Places can have addresses, telephone numbers, e-mails, websites, information about services provided, etc.

Since entering this data for as many spots as possible in the shortest possible time is "mission impossible" for one person, I definitely need a lot of help.<br>
Instructions on how to prepare this data are provided below.

### Objectives

* Implementing advanced message receiving capabilities (very limited are already present).<br> 
  The messages would be: important messages, information about events, etc.<br>
  Messages would be addressed to a specific territorial unit and would have a specific validity period.<br>
  Users would be able to choose the territorial units for which they would like to receive messages.<br>

Short term:
* Create a list of (at least) most spots providing help to refugees.<br>
  One way to achieve this would be through an extensive marketing campaign for the project.<br>
  There is no doubt that the high visibility of the project increases the number of institutions and people willing to contribute to it by several orders of magnitude.

* Provide high-quality translations.<br>
  [Let me know](mailto:adam.giergun@gmail.com) if you'd like to help me with this task.<br>
  Please start the email title with `#IfR-helpOffer:` in this case.

Long term:
* Establishing an organization that runs this project and employs people necessary for its development and maintenance.

* If it does not harm the project: make the source code available in the form of "open source" projects to ensure full transparency (application data is already released under the terms of the GNU GPL [license](https://github.com/AdamGiergun/IfR-data/blob/main/LICENSE)).

* Creating tools for entering data into the database (e.g. a convenient interface for a web browser), and API enabling access to this data through user interfaces (website, applications, plugins).

* Creation of user interfaces for other platforms (website, applications for other systems).

* Creating a website plugin to enable anyone willing to share a selected range of data from the project database on their website.

Very long term:
* Unfortunately, this refugee crisis is not the only one. I hope to turn this project into something permanent to provide help in any humanitarian crisis. <br>
  Feel free to contact me if you want to help me with this project: [my e-mail is](mailto:adam.giergun@gmail.com) - please remember to start the e-mail title with `# IfR-permanent:` .
<p align="right">(<a href="#top">back to top</a>)</p>

### Built With

* [Android Studio](https://developer.android.com/studio)

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- CONTRIBUTION -->

### Contribution

The most urgent thing would be to provide me with the best possible quality [translations](https://github.com/AdamGiergun/IfR-data#translations) and data for the application.
It is best for the data to be prepared in JSON format, in accordance with the standard proposed by me. More details below: [Data](https://github.com/AdamGiergun/IfR-data#data) <br>
It is not necessary to use Android Studio to enter this data, therefore take a look at [information about alternatives](https://github.com/AdamGiergun/IfR-data/issues/1)

### &nbsp;&nbsp;&nbsp;&nbsp;Translations
* Very good quality translations are highly needed for all README files in this repository as well as for [strings](https://github.com/AdamGiergun/IfR-data/blob/main/data/strings.xml) used in this application.

The data is divided into three types: [spot](https://github.com/AdamGiergun/IfR-data#spot), [territorial unit](https://github.com/AdamGiergun/IfR-data#territorial-unit) and [service](https://github.com/AdamGiergun/IfR-data#service).

### &nbsp;&nbsp;&nbsp;&nbsp;Spot
* The `spot` contains all the information about the place.<br>
  The `spots` data file can be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json). <br>
  Instructions can be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/), by selecting the proper `README_SPOT_<language acronym>.md`
  
### &nbsp;&nbsp;&nbsp;&nbsp;Territorial unit
* The `Territorial Unit`, is one of the properties of a place, derived from the administrative division of a given country.<br>
  For Poland, the searchable list of territorial units with identifiers is provided by the Central Statistical Office and can be found [here](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default). <br>
  As the identifiers are from an ISO 19000 based standard, I suspect other countries must use equivalent lists.<br>
  If you know where to find such lists [let me know](https://github.com/AdamGiergun/IfR-data/issues/2). <br>
  The territorial units data file can be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json). <br>
  Instructions can be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/) by selecting the proper `README_TU_<language acronym>.md`.

###  &nbsp;&nbsp;&nbsp;&nbsp;Service  
* The `Service` is simply the service offered by the given `spot`.<br>
  The service data file can be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json). <br>
  Instructions can be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/) by selecting the specific `README_SERVICE_<language acronym>.md`.
  
<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->

## Credits

* This is a place waiting for `You` :smile:

<p align="right">(<a href="#top">back to top</a>)</p>

<!-- ABOUT_ME -->

## About me

* I am an IT specialist, in recent years mainly developing my own Android application projects and self-improving in the art of programming.
  
* I have many years of experience in the IT industry, most of which is work in a small, dynamic, high-tech company, where a creative approach to projects was very important.
  I participated in many team projects. Often my work was an important (and sometimes a key) part of them, and I also ran many one-man projects for which I was fully responsible.

* In recent years, I have also had experience working in an international team dispersed in various locations, for the company [DIO-soft](http://www.dio-soft.com/en/) from Ukraine,
  contracted by a global financial corporation (unfortunately, DIO-soft lost this contract due to this corporation's concerns about Russia's aggression).
  
* In addition to practical experience, eight years ago I graduated from [Cracow University of Economics](https://uek.krakow.pl/),
  in the field of [Applied Computer Science](https://studiuj.uek.krakow.pl/listings/kierunek-informatyka-stosowana-niestarówka-i-stopien/) [(specialization Software Engineering)](https://studiuj.uek.krakow.pl/listings/specjalnosc-inzynieria-oprogramowania-niestacjonarne-i-stopien/).
  The studies were financed from the European Union funds (which was connected with increased requirements). During them, I got a scholarship for my academic performance and my final grade was "Very Good".

* When it comes to projects of social importance, I am afraid that I am "hereditary" in this direction: wink: <br>
  Two of my grandparents were very famous in their neighborhood for community service and as a result were elected to the City Council. <br>
  Both of my parents received state badges for their social activities.<br>
  As a result, there was always somewhere deep inside me a desire to try to at least equal their achievements.<br>
  I myself have been involved in various social activities over the years and creating a project like this is much more important to me than getting a well-paid job as a programmer.

* If I were to describe my other advantages, relevant to my ability to lead this project, they would be:<br>
  Extensive general knowledge (not only in the field of IT).<br>
  Creativity (my "problem" is excess, not lack of ideas).<br>
  The ability to quickly assimilate very specialized knowledge, combined with its successful application in practical solutions.<br>
  Ability to work hard and persistently in order to achieve ambitious goals.<br>
  Communicative and non-conflict, open-minded personality.
  
<p align="right">(<a href="#top">powrót</a>)</p>
