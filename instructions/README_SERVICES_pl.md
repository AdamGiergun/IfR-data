Expandable list of services is to be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json) 
```
    {
      "id": "reception",
```
 - id usługi, zaproponuj angielską nazwę dla niej.
```
      "dbType": "new",
```
 - podobnie jak w innych przypadkach "new" oznacza nowy rekord, "update" oznacza aktualizację istniejącego.
```
      "name": {
        "en": "Reception",
        "pl": "Punkt recepcyjny",
        "ru": "Стойка регистрации",
        "uk": "Прийом"
      }
    }
```
   - Mam nadzieję, że to dość oczywiste. Można użyć dowolnego akronimu języka. Pełną listę akronimów językowych można znaleźć tutaj: [List of IANA language subtags](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).
     (należy używać wartości pola "Subtag:" z wpisu oznaczonego jako "Type: language")