Examples of fulfilled territorial unit data are to be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json) 
```
    {
        "id": "PL-0264",
```
- "Territorial unit id" is one of the properties of spot coming from administrative division of country.
  For Poland searchable list of territorial units with ids is provided by Central Statistical Office, and can be found [here](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default),
  but as ids come from standard based on ISO 19000 I strongly suspect that other countries have equivalent lists.
  If you know where to find such lists [let me know](https://github.com/AdamGiergun/IfR-data/issues/2).
  Remember to not only add final units, but also their parent units,
```
        "dbType": "new",
```
  - leave it as "new", unless there's a need for updating existing record (use then "update")
``` 
        "name": {
            "en": "Wroclaw",
            "pl": "Wrocław",
            "ru": "Вроцлав",
            "uk": "Вроцлав"
    }},
```
   - I hope it's quite self-explanatory. It is possible to use any official language acronym from [List of IANA language subtags](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).
     (use "Subtag:" of "Type: language")