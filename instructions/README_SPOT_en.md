Examples of entered spot data are to be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json) 
```
{
"id": 0,
```
 - for a new record leave it as 0, I'll assign it later. But when it's an updated or aimed to be deleted record, copy existing data to be deleted or updated [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json) and use it's id.
```
"confirmed": false,
"verified": false,
```
 - leave default `false` value, it's for internal use,
```
"hasLocation": true,
```
 - information on whether there is a physical place where one can go, or whether it is only a service, for example a website, telephone line, etc.,
```
"name": {
   "en": "",
   "pl": "",
   "ru": "",
   "uk": ""
},
```
 - it's the name of the spot, my suggestion is to provide it in local language, as it may sometimes help find it easier.<br>
   In such case leave only "en" translation (it will mean "default").
```
"type": "",
```
 - presently it's for my own internal use only, it might be left empty. Current choices are: "office", "receptionPoint", but feel free to propose other options.
```
"dbType": "new",
```
 - for e new spot leave "new", otherwise use "update, or "delete" to let me know what am I supposed to do with it (remember to use existing id, as explained earlier).
```
"descriptionShort": {
   "en": "",
   "pl": "",
   "ru": "",
   "uk": ""
},
```
 - use it for providing some additional info.<br>
   As for languages, these are not limited to these in example. You can use any language acronym.<br>
   Full list of language acronyms can be found here: [List of IANA language subtags](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).<br>
   (use "Subtag:" of "Type: language" record)
```
"descriptionLong": {
   "en": "",
   "pl": "",
   "ru": "",
   "uk": ""
},
```
 - content of this field will be visible in the detailed view of a spot, and available via "more info".
```
"territorialUnitId": "",
```
 - "Territorial unit id" is one of the properties of spot coming from administrative division of country.<br>
   First of all, I would suggest [checking here](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json),
   whether the given territorial unit is not present on this list and use its `" id "` if we find it here.<br>
   For Poland searchable list of territorial units with ids is provided by Central Statistical Office, and can be found [here](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default).<br>
   As these ids come from standard based on ISO 19000 I strongly suspect that other countries have equivalent lists.<br>
   If you know where to find such lists [let me know](https://github.com/AdamGiergun/IfR-data/issues/2)
```
"location": {
```
 - any field here can be left empty if not needed
```
   "locality": "",
```
 - name of city, town, or village
```
   "street": "",
```
 - name of the street
```
   "buildingId": "",
```
 - not always a number, it can look like 12B, or F
```
   "flatOrRoomId": "",
```
 - not always a number, it can look like 12B, or F
```
   "postCode": "",
```
 - I hope it's obvious
```
   "latitude": 0.0,
   "longitude": 0.0
```
 - geographical coordinates of the spot. One of the easiest ways of finding it will be opening Google Maps, marking the spot and pressing mark icon or clicking it with mouse's right button.<br> 
   Then on computer with mouse's left button you can copy coordinates to the clipboard.
```
},
"contacts": [
```
 - if there is more then one contact for the spot multiply part included in {} separating it with commas 
```
   {
      "phone": "",
```
 - you can enter multiple phone numbers and separate them with `\n` string.
```
      "eMail": "",
      "sms": "",
      "name": "",
```
 - last position is for example for contact person name or department (if needed)
```
   "services": []
```
- use it only if there are services served only by specific contacts, look at the end for services explanation
```
   "info": {
      "en": "",
      "pl": "",
      "ru": "",
      "uk": ""
   },
```
- use it if additional info is needed for contact
```
   },
   "www": {
      "en": "",
      "pl": "",
      "ru": "",
      "uk": ""
      }
   }
],
```
- use it if there is spot's website available. If there is only one website's language version use "en" and delete the rest (and commas).
```
"services": [
   "example1",
   "example2"   
]
}
```
 - list of services' ids available at the spot.<br>
   Use if you do not fill this information for contact, or when you need to inform about the services not assigned with any contact.<br>
   List of all services is available [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json).
   If necessary, please propose additional services. [instruction here](https://github.com/AdamGiergun/IfR-data/blob/main/instructions/README_SERVICES_en.md)