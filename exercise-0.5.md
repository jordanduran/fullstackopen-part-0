```mermaid
sequenceDiagram
    participant browser
    participant server
    browser->>server: GET request html
    server->>browser: html is loaded
    browser->>server: GET css file
    server->>browser: css file is loaded
    browser->>server: GET request javascript file
    server->>browser: javascript file loaded
    // Browser starts executing javascript code to fetch JSON from server
    browser->>server: GET data.json file
    // Browser executes callback that renders the notes
```
