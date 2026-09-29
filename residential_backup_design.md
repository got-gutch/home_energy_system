# Residential Backup Power Design — 11 S Ashby Ave

```mermaid
flowchart TD
    U[Utility Service] --> MP[Main Panel]
    MP --> H[House Loads]

    OUTAGE{Primary utility power available?}
    U --> OUTAGE
    OUTAGE -- Yes --> MP

    OUTAGE -- No --> G[Firman T07573 Generator<br/>(Natural Gas)]
    G --> C[50A Cable]
    C --> I[Rear-House Coupler / Inlet]
    I --> TS[50A 10-Circuit Manual Transfer Switch<br/>(next to main panel)]
    TS --> CL[Selected Critical Circuits]
```

## Sequence

1. Utility service normally powers the main panel and house loads.
2. If primary utility power stops, deploy the Firman T07573 natural-gas generator.
3. Connect a 50A cable from the generator to the rear-house coupler/inlet.
4. The inlet feeds the 50A, 10-circuit manual transfer switch beside the main panel.
5. The transfer switch supplies the selected backup circuits.
