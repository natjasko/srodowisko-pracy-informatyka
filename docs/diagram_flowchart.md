### Diagram przepływu

```mermaid
flowchart TD
    A([START]) --> B[Uruchom aplikację]
    B --> C[Wyświetl listę zadań]
    C --> D{Czy użytkownik chce dodać zadanie?}
    D -- TAK --> E[Dodaj zadanie]
    E --> F[Zapisz]
    F --> C
    D -- NIE --> G[Zobacz plan tygodnia]
    G --> H[Wyświetl statystyki]
    H --> I([STOP])
