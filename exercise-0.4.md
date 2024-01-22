```mermaid
sequenceDiagram
    participant browser
    participant server
    browser->>server: POST request to server
    server->>browser: redirects page to headers location
    browser->>server: GET request to notes
    server->>browser: html loaded
    browser->>server: GET request main.css file
    server->>browser: css file
    browser->>server: GET request main.js file
    server->>browser: javascript file
    // Browser starts executing javascript code to fetch JSON from server
    browser->>server: GET data.json file
    // Browser executes callback that renders the notes
```
