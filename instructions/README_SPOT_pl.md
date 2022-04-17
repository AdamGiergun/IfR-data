Przykłady wypełnionych danych miejsc można znaleźć  [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json)
```
{
"id": 0,
```
- dla nowego wpisu należy pozostawić 0, numer zostanie przypisany później. Natomiest jeśli jest to zaktualizowany lub przeznaczony do usunięcia wpis, należy skopiować istniejące dane [stąd](https://github.com/AdamGiergun/IfR-data/blob/main/data/spots.json) i zmienić je pozostawiając oryginalne id.
```
"confirmed": false,
```
- należy pozostawić domyślną wartość `false`,
```
"name": "",
```
- to nazwa miejsca. Sugeruję, żeby była w języku polskim, bo czasem może to ułatwić znalezienie tego miejsca. Jeśli ktoś uważa, że przetłumaczona nazwa będzie lepszym rozwiązaniem, powinien użyć zamiast "name" - "descriptionShort", a pole "name" pozostawić puste ("")
```
"type": "office",
```
- obecnie nie używane, może w którymś momencie to wykorzystam. Aktualne opcje to: "office", "receptionPoint". Zachęcam do zaproponowania innych opcji, jeśli ktoś widzi taką potrzebę.
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
- To pole można użyć dla przetłumaczonej nazwy (jeśli jest potrzebne, jak wyjaśniłem w opisie pola "name") i/lub dodatkowych informacji.<br>
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
- pole pozostawione do wykorzystania w przyszłości na bardziej rozbudowane informacje. Jeśli ktoś uzna, że warto z niego skorzystać, to znajdę sposób na jego wyświetlenie.
```
"territorialUnitId": "",
```
- "Territorial unit id" to jedna z właściwości miejsca wywodząca się z podziału administracyjnego kraju.<br>
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
      "eMail": "",
      "sms": "",
      "name": "",
```
- imię i nazwisko osoby do kontaktu (o ile jest taka)
```
   "services": []
```
- używać go tylko wtedy, gdy są usługi obsługiwane tylko przez określone kontakty. Na końcu tej instrukcji znajduje się wyjaśnienie usług.
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
- lista identyfikatorów usług dostępnych w danej lokalizacji. Pełna lista rodzajów usług jest dostępna [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json), i można proponować dodatkowe opcje.