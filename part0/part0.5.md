sequenceDiagram
    participant Browser
    participant Server

    Browser->>Server: GET /spa
    Server-->>Browser: HTML
    Browser->>Server: GET /spa.js
    Browser->>Server: GET /main.css
    Browser->>Server: GET /data.json
    Server-->>Browser: Notes JSON
    Browser->>Browser: Render notes
