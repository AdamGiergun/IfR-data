Examples of fulfilled territorial unit data are to be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json) 
```
    {
        "id": "PL-1261",
```
- "Territorial unit id" is one of the properties of spot coming from administrative division of country.<br>
  For Poland searchable list of territorial units with ids is provided by Central Statistical Office, and can be found [here](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default).<br>
  As these ids come from standard based on ISO 19000 I strongly suspect that other countries have equivalent lists.<br>
  If you know where to find such lists [let me know](https://github.com/AdamGiergun/IfR-data/issues/2).
  Remember to not only add final units, but also their parent units,
```
        "dbType": "new",
```
  - leave it as "new", unless there's a need for updating existing record (use then "update")
``` 
      "name": {
        "en": "Kraków",
        "pl": "Kraków",
        "ru": "Краков",
        "uk": "Краків"
        },
```
   - I hope it's quite self-explanatory. It is possible to use any official language acronym from [List of IANA language subtags](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).<br>
     (use "Subtag:" of "Type: language")
```
      "geoLocation":{
        "latitude": 0.0,
        "longitude": 0.0
      }
    },
```
   - geographical coordinates of the territorial unit. My proposal is a choice of something like the location of the central point of the largest city in this territorial unit, not in its geographical center.<br>
     One of the easiest ways of finding it will be opening Google Maps, marking the spot and pressing mark icon or clicking it with mouse's right button.<br>
     Then on computer with mouse's left button you can copy coordinates to the clipboard.
     . 