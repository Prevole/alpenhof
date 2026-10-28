# Maquette Alpenhof

A model railway lighting project featuring individually controlled LED lighting for buildings and scenery.

## Architecture

- **Controller:** Raspberry Pi Pico 2 WH generates control signals.
- **LED Drivers:** ULN2803A ICs switch each LED independently on the ground side.
- **LED Hub:** Custom KiCad PCB distributes power and connects up to 16 LEDs via JST-XH connectors.
- **Power:** External 15V DC supply powers the LEDs independently of the Pico.
- **Interconnection:** A 20-pin IDC ribbon cable carries 16 individual LED channels and four shared +15V connections between the controller and hub.

The Pico controls the drivers; it does not supply power directly to the LEDs. All circuits share a common ground.

## Status

Work in progress.
