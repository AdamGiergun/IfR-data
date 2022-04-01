Examples of fulfilled spot data are to be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json) 

{
"id": "0",
 - for a new record leave it as 0, I'll assign it later. But when it's an updated or aimed to be deleted record, copy existing data to be deleted or updated [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json) and use it's id.

"name": "",
 - it's the name of the spot, my suggestion is to provide it in local language, as it may sometimes help find it easier. If you think that translated name will be a better solution use "descriptionShort" instead, and leave "name" empty ("")

"type": "office",
 - presently it's for my own internal use, maybe at some point I'll make some use of it. Current choices are: "office", "receptionPoint", but feel free to propose other options.

"dbType": "new",
 - for e new spot leave "new", otherwise use "update, or "delete" to let me know what am I supposed to do with it (remember to use existing id, as explained earlier).

"descriptionShort": {
"en": "",
"pl": "",
"ru": "",
"uk": ""
},
 - use it for translated name (as explained in "name"), or some additional info. As for languages, these are not limited to these in example. You can use any acronym.
   Full list of language acronyms can be found here: [List of IANA language subtags](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).
   (use "Subtag:" of "Type: language")

"descriptionLong": {
"en": "",
"pl": "",
"ru": "",
"uk": ""
},
 - field left for future use for some elaborate info, feel free to use it, I'll find the way of displaying it. 

"territorialUnitId": "PL-1465",


"location": {
"locality": "",
"street": "",
"buildingId": "",
"flatOrRoomId": "",
"postCode": "",
"latitude": "0.0",
"longitude": "0.0"
},
"contacts": [
{
"phone": "+48477217575",
"eMail": "",
"sms": "",
"name": "",
"services": [],
"www": {
"en": "https://www.gov.pl/web/mswia/informacja-dla-uchodzcow-z-ukrainy",
"pl": "https://www.gov.pl/web/mswia/informacja-dla-uchodzcow-z-ukrainy",
"ru": "https://www.gov.pl/web/mswia/informacja-dla-uchodzcow-z-ukrainy",
"uk": "https://www.gov.pl/web/mswia/informacja-dla-uchodzcow-z-ukrainy"
}
}
],
"services": [
"information"
]
}