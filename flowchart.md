```mermaid
flowchart TD
    A[Customer purchases air conditioner] --> B[Installer offers 5-year warranty]
    B --> C[Customer agrees and shares details via app]
    C --> D[Company receives details]
    D --> E[Send email to customer<br>for warranty confirmation]
    E --> F[Customer clicks link<br>and confirms details on webform]
    F --> G{Optional: Customer opts-in<br>for marketing emails}
    G -- Yes --> H[Suggest downloading<br>Tadiran IoT app]
    G -- No --> H
    H --> I[Display thank-you message<br>and confirm warranty]

    %% Styling
    classDef box fill:#f9f9f9,stroke:#333,stroke-width:2;
    classDef diamond fill:#f1f1c1,stroke:#333,stroke-width:2;
    class A,B,C,D,E,F,H,I box;
    class G diamond;
