# Part 0 – Notes App Diagrams

## Exercise 0.4 – New note (Traditional app)

```mermaid
sequenceDiagram
    participant Browser
    participant Server

    Browser->>Server: POST /new_note
    Server->>Server: Save note
    Server-->>Browser: Redirect to /notes
    Browser->>Server: GET /notes
    Server-->>Browser: Updated HTML
