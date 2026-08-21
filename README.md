# blocks

**Experimental verifier and distributed-systems research for Bitopia.**

> **Status: prototype / research.** This repository explores distributed verification of machine-generated telemetry and future Bitopia consensus mechanisms. It is not a production blockchain, does not currently provide post-quantum security, and does not make guarantees about geographic proof, 51% resistance, or renewable-energy provenance.

## Current technical baseline

The current Rust dependency set includes:

- SHA-3 / Keccak hashing through `sha3`.
- Ed25519 signatures through `ed25519-dalek`.
- Tokio for asynchronous execution.
- libp2p for peer-to-peer networking experiments.
- Serde / JSON for data interchange.
- Chrono for timing and timestamp utilities.

**Post-quantum signatures are a roadmap item, not a current implementation claim.** A future migration should be documented only after the selected primitive is implemented, backed by test vectors, interoperable, and reviewed.

## Axiom integration

Axiom is Bitaris Labs' secure energy-attestation hardware research track. It begins with physical electrical generation measurement at the edge.

The present Axiom breadboard is a functional/provisioning prototype using an ESP32-C3, INA226 metrology, and an ATECC608B secure element. Production hardware-rooted telemetry signing and the final isolated architecture remain under development.

Do not assume that the secure element itself performs metrology or independently polls the sensor. The ATECC608B is a cryptographic device on the I2C interface; the final trust-boundary architecture must account for that constraint.

## Energy evidence

The research target is evidence derived from **integrated electrical energy (Wh)**, not instantaneous power alone. Future $EW/e-watt accounting may consume eligible attested Wh measurements after renewable-source and anti-fraud controls are defined.

Hardware signatures can strengthen device-origin and integrity evidence. They do not, by themselves, prove that the measured source was renewable.

## Research directions

- Hardware-rooted telemetry verification.
- Renewable-energy provenance and $EW/e-watt accounting.
- Peer-to-peer verification and distributed state.
- Explicit threat models for any Proof-of-Energy or space-time/location evidence.
- Post-quantum signature migration after implementation and validation.
- Long-horizon autonomous infrastructure, including orbital/off-world environments.

## Build

```bash
git clone https://github.com/Bitopia-DUNA/blocks.git
cd blocks
cargo build --release
```

Any simulator should be labeled according to what it actually tests. Do not describe a software-only simulation as validating Axiom hardware signatures until the real hardware-attestation path is connected and verified.

## Project status language

Use these labels consistently:

- **Demonstrated** - observed on real hardware/software.
- **Under development** - implemented partially or currently being validated.
- **Research / proposed** - architecture, cryptography, governance, or economic mechanisms not yet implemented and verified.

**Physics first. Evidence second. Networks coordinate.**
