```mermaid

sequenceDiagram
    participant browser
    participant server

    browser->>server: get notes
    activate server
    server->>browser: notes
    deactivate server
    
    activate browser
    browser-->browser: render notes
    deactivate browser

    browser->>server: add note
    activate server
    server->>browser: refresh page
    deactivate server

```