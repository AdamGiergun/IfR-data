Przykłady wypełnionych danych miejsc można znaleźć  [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json)
```
{
"id": 0,
```
- dla nowego wpisu należy pozostawić 0, numer zostanie przypisany później. Natomiest jeśli jest to zaktualizowany lub przeznaczony do usunięcia wpis, należy skopiować istniejące dane [stąd](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json) i zmienić je pozostawiając oryginalne id.
```
"confirmed": false,
"verified": false,
```
- należy pozostawić domyślną wartość `false`,
```
"name": {
   "en": "",
   "pl": "",
   "ru": "",
   "uk": ""
},
```
- nazwa miejsca. Sugeruję, żeby była w języku polskim, bo czasem może to ułatwić znalezienie tego miejsca.<br>
  W takim wypadku należy nazwę wpisać w pole "en" (w tym wypadku będzie to oznaczać wartość domyślną), a resztę pól usunąć.
```
"type": "",
```
- obecnie nie używane, można pozostawić puste. Aktualne opcje to: "office", "receptionPoint". Zachęcam do zaproponowania innych opcji, jeśli ktoś widzi taką potrzebę.
```
"dbType": "new",
```
- dla nowego wpisu należy pozostawić "new", w innych przypadkach należy użyć "update lub "delete", aby dać mi znać, co mam z tym wpisem zrobić (należy pamiętać, aby użyć istniejącego id, jak wyjaśniłem to powyżej).
```
"descriptionShort": {
   "en": "",
   "pl": "",
   "ru": "",
   "uk": ""
},
```
- To pole można użyć dla umieszczenia dodatkowych informacji.<br>
  Jeśli chodzi o języki, nie ograniczają się one do tych z przykładu. Można użyć dowolnego akronimu języka.<br>
  Pełną listę akronimów językowych można znaleźć tutaj: [List of IANA language subtags](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).<br>
  (należy używać wartości pola "Subtag:" z rekordu oznaczonego jako "Type: language")
```
"descriptionLong": {
   "en": "",
   "pl": "",
   "ru": "",
   "uk": ""
},
```
- pole będzie wyświetlane w widoku szczegółowym punktu (dostępnym przez przycisk "więcej").
```
"territorialUnitId": "",
```
- "Territorial unit id" to jedna z właściwości miejsca wywodząca się z podziału administracyjnego kraju.<br>
  W pierwszy rzędzie prosiłbym [sprawdzić tu](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json),
  czy dana jednostka terytorialna nie jest obecna na tej liście i użyć jej `"id"`, jeśli ją tu znajdziemy.<br>
  Dla Polski przeszukiwalny wykaz jednostek terytorialnych wraz z identyfikatorami dostarcza GUS i można go znaleźć [tutaj](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default).<br>
  Ponieważ identyfikatory stworzone są na podstawie standardu ISO 19000, podejrzewam, że inne kraje mają równoważne listy.<br>
  Jeśli wiesz, gdzie znaleźć takie listy [daj mi znać](https://github.com/AdamGiergun/IfR-data/issues/2)
```
"location": {
```
- any field here can be left empty if not needed- każde pole tutaj można pozostawić puste, jeśli nie jest potrzebne.
```
   "locality": "",
```
- nazwa miasta, miejscowości lub wsi,
```
   "street": "",
```
- nazwa ulicy,
```
   "buildingId": "",
```
- nie zawsze będzie to liczba, przykładowo może to być też 12B lub F,
```
   "flatOrRoomId": "",
```
- nie zawsze będzie to liczba, przykładowo może to być też 12B lub F,
```
   "postCode": "",
```
- mam nadzieję, że to oczywiste,
```
   "latitude": 0.0,
   "longitude": 0.0
```
- współrzędne geograficzne miejsca. Jednym z najłatwiejszych sposobów ich odnalezienia będzie wejście na Google Maps, zaznaczenie miejsca i naciśnięcie ikonki zaznaczenia lub kliknięcie jej prawym przyciskiem myszy.<br>
  Następnie na komputerze lewym przyciskiem myszy można skopiować wyświetlone współrzędne do schowka.
```
},
"contacts": [
```
- jeśli jest więcej niż jeden kontakt dla adresu można powielić część zawartą w {} oddzielając kolejne wpisy przecinkami.
```
   {
      "phone": "",
```
 - można wprowadzić wiele numerów telefonów i oddzielić je spacją.
```
      "eMail": "",
      "sms": "",
      "name": "",
```
- ostatnia pozycja to n.p. imię i nazwisko osoby do kontaktu lub wydział (wypełniamy tylko jeśli to potrzebne).
```
   "services": []
```
- używać go tylko wtedy, gdy są usługi obsługiwane tylko przez określone kontakty/wydziały. Na końcu tej instrukcji znajduje się wyjaśnienie usług.
```
   "info": {
      "en": "",
      "pl": "",
      "ru": "",
      "uk": ""
   },
```
 - używać jeśli potrzebne jest umieszczenie dodatkowych informacji dla kontaktu
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
- do użycia, jeśli dostępna jest strona internetowa lokalizacji. Jeśli jest tylko jedna wersja językowa tej strony, należy użyć pola "en" i usunąć resztę (wraz z przecinkami).
```
"services": [
   "example1",
   "example2"   
]
}
```
- lista identyfikatorów usług dostępnych w danej lokalizacji.<br>
  Używać jeśli nie wypełniamy tej informacji dla kontaktu, lub gdy potrzebne jest poinformowanie o usługach nieprzypisanych do żadnego konkretnego kontaktu.<br>
  Pełna lista rodzajów usług jest dostępna [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json).<br>
  W razie potrzeby proszę zaproponować dodatkowe usługi. [Instrukcja tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/instructions/README_SERVICES_pl.md)