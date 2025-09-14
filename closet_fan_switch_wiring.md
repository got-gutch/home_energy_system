# Wiring Diagram & Guidance: Shelly 1PM Gen3 Smart Switch for Attic Fan (Closet Switch Box)

![Switch Box Reference](image1)

## Components
- Shelly 1PM Gen3 Smart Relay Switch
- Standard fan switch (toggle or rocker, right switch in closet)
- Closet switch box (see image above)
- AC wiring: Hot (black), Neutral (white), Load (to fan), Ground (bare/green)
- Extra 14 AWG or 12 AWG wire for pigtails (recommend pre-cut pigtails)

---

## What’s Visible in Your Switch Box

- **Two switches:** The right switch is for your fan.
- **White wires:** Two visible, likely neutrals or possibly used as switch legs. Should be confirmed with a voltage tester.
- **No visible black/hot wires:** Likely attached to the switches or tucked in the box.
- **No visible ground wire:** May be attached to the box (if metal) or hidden behind the switches.

---

## Steps Before Wiring

1. **Turn off power at the breaker.**
2. **Pull both switches fully out of the box** to expose all wires.
3. **Identify:**
   - **Black/hot wire(s)**
   - **White/neutral wire(s)** (should be in a bundle if neutral is present)
   - **Load wire** (to fan)
   - **Ground wire** (bare copper or green, may be attached to box or behind switches)
4. **Check with a voltage tester or multimeter** to confirm which wires are hot, neutral, and load.

---

## Wiring Diagram

```
Closet Switch Box:                Shelly 1PM Gen3:          Fan:

+------------------+              +------------------+      +------------------+
|                  |              | L (Line)   <---->|      |                  |
|   Black (Hot)    |--------------|                  |      |                  |
|                  |              | N (Neutral)<---->|      |                  |
|   White (Neutral)|--------------|                  |      |                  |
|                  |              | O (Output)------>|------|   Fan (Load)     |
|   Load to Fan    |<-------------|                  |      |                  |
|                  |              | SW (Switch) <----|------|   Manual Switch  |
|   Ground         |--------------| G (Ground) <---->|      |                  |
+------------------+              +------------------+      +------------------+
```

---

## Installation Steps

1. **Turn off power at the breaker.**
2. **Remove the switch cover and gently pull out the switch.**
3. **Identify wires as described above.**
4. **Shelly wiring:**
   - **L (Line):** Connect to black (hot) wire.
   - **N (Neutral):** Connect to white (neutral) wire. If not present, you’ll need to run a new neutral wire from a nearby outlet or junction box.
   - **O (Output):** Connect to the wire going to the fan (load).
   - **SW (Switch):** Connect to one terminal of the manual switch (the other terminal should connect to Line).
   - **G (Ground):** Connect to ground wire if present, or to the metal box if bonded.
5. **Use extra pigtail wires** as needed for secure connections.
6. **Tuck the Shelly 1PM into the box behind the switch. Reinstall the switch and cover.**
7. **Restore power and test manual and app control.**
8. **Set up Shelly 1PM Gen3 in the app and configure automation as desired.**

---

## Notes

- Use wire nuts and electrical tape for secure connections.
- Make sure the box has enough space for the Shelly device.
- Confirm wiring matches Shelly 1PM Gen3 instructions (see manufacturer documentation).
- If neutral is not present, you’ll need extra wire and potentially an electrician’s help.
- Always comply with local electrical codes.

---

## Shopping List

- 14 AWG (15A circuit) or 12 AWG (20A circuit) solid copper wire pigtails
- Wire nuts
- Electrical tape

---

If you need help identifying wires after pulling the switches out, let me know and send a photo!