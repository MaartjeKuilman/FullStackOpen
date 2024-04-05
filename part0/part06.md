```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/spa/new_note_spa
    activate server
    server-->>browser: [201] HTML created
    deactivate server

    Note right of browser: The browser stays on the same page and sends no further HTTP requests
```
