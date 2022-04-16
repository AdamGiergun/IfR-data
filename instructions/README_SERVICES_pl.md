Expandable list of services is to be found [here](https://github.com/AdamGiergun/IfR-data/blob/main/data/services.json) 
```
    {
      "id": "basicMedicalAssistance",
```
 - id usługi, zaproponuj angielską nazwę dla niej.
```
      "dbType": "new",
```
 - podobnie jak w innych przypadkach "new" oznacza nowy rekord, "update" oznacza aktualizację istniejącego.
```
      "name": {
        "en": "Basic medical assistance",
        "pl": "Podstawowa opieka medyczna",
        "ru": "Основная медицинская помощь",
        "uk": "Основна медична допомога"
      },
```
 - Mam nadzieję, że to dość oczywiste. Można użyć dowolnego akronimu języka. Pełną listę akronimów językowych można znaleźć tutaj: [List of IANA language subtags](https://www.iana.org/assignments/language-subtag-registry/language-subtag-registry).<br>
   (należy używać wartości pola "Subtag:" z wpisu oznaczonego jako "Type: language")
```
      "keywords": {
        "en": "Doctor, Nurse, Health",
        "pl": "lekarz, pielęgniarz, pielęgniarka, zdrowie",
        "ru": "Доктор, медсестра, здоровье",
        "uk": "Доктор, медсестра, здоров'я"
      }
    }
```
- słowa kluczowe nie są widoczne dla użytkowników, ale pomagają w wyszukiwaniu miejsc.