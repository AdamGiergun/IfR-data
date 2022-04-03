Przykłady wpisów jednostek terytorialnych można znaleźć [tutaj](https://github.com/AdamGiergun/IfR-data/blob/main/data/territorialUnits.json) 
```
    {
        "id": "PL-0264",
```
- - "Territorial unit id" to jedna z właściwości miejsca wywodząca się z podziału administracyjnego kraju.
    Dla Polski przeszukiwalny wykaz jednostek terytorialnych wraz z identyfikatorami dostarcza GUS i można go znaleźć [tutaj](https://eteryt.stat.gov.pl/eTeryt/rejestr_teryt/udostepnianie_danych/baza_teryt/uzytkownicy_indywidualni/wyszukiwanie/wyszukiwanie.aspx?contrast=default).
    Ponieważ identyfikatory stworzone są na podstawie standardu ISO 19000, podejrzewam, że inne kraje mają równoważne listy.
    Jeśli wiesz, gdzie znaleźć takie listy [daj mi znać](https://github.com/AdamGiergun/IfR-data/issues/2).
```
        "dbType": "new",
```
  - należy pozostawić to jako "new", chyba że istnieje potrzeba aktualizacji istniejącego wpisu (wtedy będzie to "update")
```
        "name": {
            "en": "Wroclaw",
            "pl": "Wrocław",
            "ru": "Вроцлав",
            "uk": "Вроцлав"
    }}
```
   - Mam nadzieję, że to dość oczywiste. Można użyć dowolnego akronimu języka. Pełną listę akronimów językowych można znaleźć tutaj: [List of IANA language subtags](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).
     (należy używać wartości pola "Subtag:" z wpisu oznaczonego jako "Type: language")