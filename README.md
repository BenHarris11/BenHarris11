# Hi, I'm Ben Harris

Computer Engineering student at Cal Poly San Luis Obispo,
graduating Spring 2028. I build embedded firmware and the protocols and apps
around it — currently the sole engineer behind **Kyntex**, a wearable-sensing
startup I co-founded.

## What I'm building

**[Kyntex](https://github.com/Kyntex-org/Kyntex)** — a wearable platform for
training telemetry you can actually trust. Most wearables show attractive
charts without answering whether the device was fitted correctly or whether a
session was captured without silent data loss. I designed and built the whole
stack to answer both:

- **Firmware** — Nordic nRF54L15 running Zephyr RTOS: event-driven IMU
  acquisition, band-fit sensing, battery monitoring, and an on-device workout
  engine that classifies activity and counts steps, jumps, and mechanical load
- **Protocol** — a custom, versioned binary BLE contract with checksums and
  recording-integrity counters (boot ID, session ID, packet/sample sequence,
  dropped-sample accounting), kept in lockstep across three implementations
- **Applications** — a native SwiftUI/CoreBluetooth iOS app and a
  dependency-free Web Bluetooth dashboard, both decoding the same device data
- **Hardware** — schematic and PCB design in KiCad/Altium, fabrication, and
  bench bring-up of a custom NINA-B302/nRF52 board

Take a look at the public, hardware-free portfolio:
**[Kyntex-Technical-Public](https://github.com/Kyntex-org/Kyntex-Technical-Public)**
— firmware-core modules with unit tests, and a dashboard demo that runs with no
band, no Bluetooth, and no server.

I'm also running a smaller research testbench,
**Passive Tendon-Response Sensing**, exploring whether a landing can passively
excite the patellar tendon in a way an accelerometer can detect — early-stage,
honestly scoped, and not a claim about injury risk or diagnosis.

## Technical toolbox

`C` `C++` `Python` `Zephyr RTOS` `nRF Connect SDK` `Nordic nRF54L15 / nRF52`
`STM32` `BLE GATT` `SPI` `I2C` `UART` `ADC` `KiCad` `Altium` `SwiftUI`
`CoreBluetooth` `Web Bluetooth` `Git`

## Elsewhere

- [LinkedIn](https://linkedin.com/in/benjaharris)
- [Kyntex-org](https://github.com/Kyntex-org) — the organization behind Kyntex

---
*Kyntex is an engineering prototype, not a medical device. It is not intended
to diagnose, treat, prevent, or predict injury.*
