# ⬛ blocks Layer-1: The Zero-Trust Orbital Ledger
**The Decentralized Post-Quantum Protocol Powering the Sovereign Space Economy.**
*Language: Rust (Space-Grade Memory Safety) | Firmware: Zephyr RTOS | Security: NIST Post-Quantum*

## 🌌 Overview
`blocks` is the uncompromising, zero-server Layer-1 blockchain architecture that underpins the Bitopia Network State and the dasOS terminal. It is designed specifically to eradicate terrestrial cloud OpEx, prevent 51% state-actor attacks, and execute high-margin protocol economics for aerospace primitives. 

We do not use Proof-of-Work or Proof-of-Stake. The `blocks` network is secured by **Proof-of-Space-Time (PoST)** and **Proof-of-Energy (PoE)**, tethering cryptographic truth directly to the immutable laws of thermodynamics and orbital physics.

---

## ⚙️ The Consensus Engine (PoST + PoE)
To forge a block on this network, a node must cryptographically prove two physical realities:
1. **Proof of Energy (PoE):** The hardware must physically capture and attest to the generation of thermodynamic energy ($EW).
2. **Proof of Space-Time (PoST):** The node's telemetry latency must fall within strict orbital parameters (e.g., `min_orbital_latency_ms: 45`, `max_orbital_latency_ms: 120`), mathematically preventing terrestrial VPN routing or data center spoofing.

---

## 🛡️ Core Architecture & Modules

### 1. The Hardware Forge (`axiom-c-firmware`)
Built on **Zephyr RTOS**, the Axiom firmware interfaces with Microchip ATECC608B Secure Enclaves. Energy metrology (MWh) is captured, hashed, and signed strictly *inside* the tamper-proof silicon. Private keys never leave the enclave.

### 2. Post-Quantum Cryptography (`blocks-consensus`)
Securing multi-billion dollar aerospace assets requires immunity to Shor's and Grover's algorithms. The core L1 engine utilizes:
* **Keccak-512 / SHA-512** for state hashing.
* **CRYSTALS-Dilithium** lattice-based signatures for hardware telemetry verification.

### 3. The Galactic Registry (`registry-tax-engine`)
The smart-contract layer handling the financial logic of the space economy. It manages:
* Decentralized Sovereign DAO Formation.
* Immutable Intellectual Property hashing.
* **Celestial Claims:** Staking and claiming lunar/orbital physical coordinates.
* **RWA Tokenization:** Fractionalizing multi-million dollar aerospace assets into liquid, tradable shares.

### 4. The Network Mesh (`swarm-mesh`)
The nervous system of the Axiom Swarm. It ingests zero-knowledge citizen transactions and live hardware telemetry, compiling valid synapses into Merkle Roots for L1 block compression.

### 5. Sovereign Habitat Governance (`governance-engine`)
Manages Zero-Knowledge (ZK) citizen onboarding, risk clearances, and dynamic thermal capacity limits for individual orbital sectors. 

---

## 🚀 Bootstrapping the L1 

To compile and test the Post-Quantum consensus engine locally:

```bash
# Clone the repository
git clone [https://github.com/bitaris/blocks.git](https://github.com/joematopia/blocks.git)
cd blocks

# Build the Rust kernel
cargo build --release

# Run the L1 Simulator (Tests PoST and Axiom Enclave Signatures)
cargo run --bin consensus_engine
```

## 📖 The Bitopia Ecosystem

This repository is the core ledger. To view the frontend interface or the founding protocols, visit the broader ecosystem:

* 👉 **[dasOS Interface](https://github.com/joematopia/dasOS):** The Space Economy Terminal.
* 👉 **[The Bitopia Codex](https://github.com/joematopia/Bitopia):** The Founding Laws and Tokenomics. 

**Code is Law. Physics is Truth. Trust the Enclave.**
