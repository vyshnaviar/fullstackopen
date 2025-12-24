sequenceDiagram
    participant Browser
    participant Server

    Browser->>Browser: User writes note
    Browser->>Server: POST /new_note_spa (JSON)
    Server->>Server: Save note
    Server-->>Browser: 201 Created
    Browser->>Browser: Update UI
