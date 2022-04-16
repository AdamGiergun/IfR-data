Expandable list of services is to be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json) 
```
    {
      "id": "basicMedicalAssistance",
```
 - id for service, propose english name for it
```
      "dbType": "new",
```
 - as in other cases, "new" is for a new record, "update" for updated   
```
      "name": {
        "en": "Basic medical assistance",
        "pl": "Podstawowa opieka medyczna",
        "ru": "Основная медицинская помощь",
        "uk": "Основна медична допомога"
      },
```
 - I hope it's quite self-explanatory. It is possible to use any official language acronym from [List of IANA language subtags](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).<br>
  (use "Subtag:" of "Type: language")
```
      "keywords": {
        "en": "Doctor, Nurse, Health",
        "pl": "lekarz, pielęgniarz, pielęgniarka, zdrowie",
        "ru": "Доктор, медсестра, здоровье",
        "uk": "Доктор, медсестра, здоров'я"
      }
    }
```
- keywords are not visible to users, but help in searching for spots.
