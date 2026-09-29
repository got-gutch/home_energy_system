# Residential Backup Power Design — 11 S Ashby Ave

```mermaid
flowchart TD
    U[Utility Service] --> MP[Main Panel]
    MP --> H[Non-Backup House Loads]

    OUTAGE{Primary utility power available?}
    U --> OUTAGE
    OUTAGE -- Yes --> MP

    OUTAGE -- No --> G[Firman T07573 Generator<br/>(Natural Gas)]
    G --> C[50A Cable]
    C --> I[VEVOR CS6375 Power Inlet Box<br/>(or similar)]
    I --> TS[VEVOR 50A 10-Circuit Manual Transfer Switch<br/>NEMA 3R, Double-Throw, Watt Meter<br/>(or similar)]
    MP --> TS
    TS --> CL[Selected Backup Circuits]
```

## Sequence

1. Utility service normally powers the main panel and house loads.
2. If primary utility power stops, deploy the Firman T07573 natural-gas generator.
3. Connect a 50A cable from the generator to the rear power inlet box (CS6375 style).
4. The inlet feeds the 50A, 10-circuit manual transfer switch kit (VEVOR or similar) located beside the main panel.
5. Add/confirm the required feeder/control wiring from the transfer switch back to the main panel so each selected branch circuit can be switched between utility and generator.
6. During outage mode, the transfer switch supplies only the selected backup circuits.

## Proposed Backup Circuit Set (to Confirm at Panel)

Prioritize existing must-run loads from `/home/runner/work/home_energy_system/home_energy_system/electrical_information.md`:

1. Refrigerator circuit
2. Home networking circuit (modem/router/switch)
3. Gas furnace blower/controls circuit
4. Air-conditioner critical control/air-handler circuit (if compatible with transfer switch and generator capacity)

Then fill remaining transfer-switch positions with high-value essentials, such as:

5. Kitchen small-appliance circuit (minimum one)
6. Basement/utility lighting circuit
7. Sump pump circuit (if present)
8. Boiler/ignition or hydronic controls (if separate from furnace controls)
9. Essential receptacles circuit (office/charging/medical devices)
10. Safety/security circuit (garage door opener / alarm / exterior lighting as needed)

## Circuit Identification and Validation Checklist

- Confirm each candidate breaker number and amperage in the Siemens main panel.
- Verify transfer switch circuit amp limits and pole requirements (120V single-pole vs any 240V/tied loads).
- Validate Firman T07573 available running watts against simultaneous selected loads.
- Mark final selected circuits in the transfer switch schedule and panel directory.
- Have a licensed electrician confirm code-compliant wiring and interconnection details before installation.
