```mermaid
sequenceDiagram;
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
    activate server
    server-->>browser: 201 created
    deactivate server

    Note right of browser: The server saves the note according to the HTTP POST request
```
