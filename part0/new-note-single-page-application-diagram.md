```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 Created (new note saved)
    deactivate server

    Note right of browser: The browser updates the UI dynamically with the new note, without refreshing the page
```
