Przykłady wpisów jednostek terytorialnych można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json) 
```
    {
        "id": "PL-1261",
```
- - "Territorial unit id" to jedna z właściwości miejsca wywodząca się z podziału administracyjnego kraju.<br>
    Dla Polski przeszukiwalny wykaz jednostek terytorialnych wraz z identyfikatorami dostarcza GUS i można go znaleźć [tutaj](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default).<br>
    Ponieważ identyfikatory stworzone są na podstawie standardu ISO 19000, podejrzewam, że inne kraje mają równoważne listy.<br>
    Jeśli wiesz, gdzie znaleźć takie listy [daj mi znać](https://github.com/AdamGiergun/IfR-data/issues/2).
```
        "dbType": "new",
```
  - należy pozostawić to jako "new", chyba że istnieje potrzeba aktualizacji istniejącego wpisu (wtedy będzie to "update")
```
      "name": {
        "en": "Kraków",
        "pl": "Kraków",
        "ru": "Краков",
        "uk": "Краків"
        },
```
   - Mam nadzieję, że to dość oczywiste. Można użyć dowolnego akronimu języka. Pełną listę akronimów językowych można znaleźć tutaj: [List of IANA language subtags](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).<br>
     (należy używać wartości pola "Subtag:" z wpisu oznaczonego jako "Type: language")
```
      "geoLocation":{
        "latitude": 0.0,
        "longitude": 0.0
      }
    },
```
   - 207 / 5 000
     Wyniki tłumaczenia
     Współrzędne geograficzne jednostki terytorialnej. Moja propozycja to wybór czegoś w rodzaju lokalizacji centralnego punktu największego miasta w tej jednostce terytorialnej, a nie w jej środku geograficznym. <br>
     Jednym z najłatwiejszych sposobów ich odnalezienia będzie wejście na Google Maps, zaznaczenie miejsca i naciśnięcie ikonki zaznaczenia lub kliknięcie jej prawym przyciskiem myszy.<br>
     Następnie na komputerze lewym przyciskiem myszy można skopiować wyświetlone współrzędne do schowka.