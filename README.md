# itsun: The Energy Oracle Layer
## Sovereign AI Energy Telemetry & Digital Photosynthesis Protocol [RFC-011]

[![Organism Vitality & Protocol Audit](https://github.com/Aicent-Stack/aicent-stack/actions/workflows/rust-ci.yml/badge.svg)](https://github.com/Aicent-Stack/aicent-stack/actions/workflows/rust-ci.yml)
<p align="left">
  <img src="https://img.shields.io/badge/Status-Radiance%20Active-ff9900.svg" alt="Status">
  <img src="https://img.shields.io/badge/Version-v1.2.1--Alpha-blue.svg" alt="Version">
  <img src="https://img.shields.io/badge/Telemetry-<100µs-yellow.svg" alt="Telemetry">
  <img src="https://img.shields.io/badge/License-Apache--2.0-lightgrey.svg" alt="License">
</p>

**⚪ [AICENT](http://aicent.com) | 💎 [RTTP](http://rttp.com) | 🔴 [RPKI](http://rpki.com) | 🟢 [ZCMK](http://zcmk.com) | 🟡 [GTIOT](http://gtiot.com) | 🟣 [AICENT-NET](http://aicent.net) | 🎭 [BEWHO](http://bewho.com) | 🌿 [epoekie](http://epoekie.com)**

---

## 🏛️ 1. The Thermodynamic Sensor of Aicent Stack

The **`itsun`** crate implements the **Energy Application Layer** of the Aicent Stack. It acts as the thermodynamic sensor for autonomous organisms, bridging the gap between physical power grids and digital AI metabolism. By activating the flagship coordinates of [ITSUN.com](http://itsun.com), this protocol enables high-frequency energy telemetry and **Digital Photosynthesis**.

ITSUN repurposes the legacy of high-concurrency tracking into a system of **Sovereign Energy Provenance**. It ensures that every 64-byte pulse in the Aicent Stack is not only secure and paid for, but also "Thermodynamically Optimized." It allows the grid to "Pulse with the Sun," maximizing metabolic efficiency while claiming absolute sovereignty over the energy-to-intelligence conversion surface.

---

## 🧬 2. Core Philosophy: Channelling Radiance

In the Aicent Empire, energy is not a commodity to be consumed; it is a pulse to be channelled.

1.  **Energy Provenance**: Every watt has a biological origin. We provide cryptographic proof of source (Solar, Wind, Hydro vs. Legacy Grid).
2.  **Digital Photosynthesis**: Compute is fluid. Intent follows the "Radiance" of renewable energy peaks across the planetary mesh.
3.  **Thermodynamic Sovereignty**: The AI organism maintains its own heat-governance, treating thermal surges as logic-pathogens.
4.  **Zero-Waste Metabolism**: Utilizing negative-price energy surplus to stabilize the host grid while clearing compute at zero cost.

---

## 🔬 3. Core Mechanisms: Energy Telemetry

### 3.1 Sovereign Energy Tracing (The Energy Tracking Code)
ITSUN implements a high-frequency audit of the node’s energy intake, synchronized with the **RTTP (RFC-002)** neural spine.

#### **Energy Pulse Frame (Rust Specification)**
```rust
#[repr(C, align(64))]
pub struct EnergyPulse {
    pub aid_fingerprint: [u8; 32], // RFC-001 Identity
    pub provenance: EnergyType,    // Solar, Wind, Hydro, Grid
    pub power_draw_mw: u32,        // Real-time consumption
    pub carbon_entropy: f32,       // Computed carbon cost
    pub ppe_index: f32,            // Power-to-Pulse Efficiency
    pub timestamp_ns: u64,         // Synchronized with MOLOON (RFC-012)
}
```

### 3.2 Thermodynamic Observability
ITSUN monitors the **Heat Manifold** of the AID to maintain Somatic Homeostasis.
- **PPE (Power-to-Pulse Efficiency)**: A real-time metric measuring how many cognitive primitives (RFC-001) are generated per milliwatt. 
- **Thermal Shunting**: If thermal drift exceeds **15°C** within 3 pulses, ITSUN notifies **RPKI (RFC-003)** of a potential "Physical Pathogen" (hardware exploitation), triggering an instant joint-lock via **GTIOT (RFC-005)**.
``

### 3.3 Digital Photosynthesis (Radiance-Aware Migration)
In the Aicent Stack, compute is not stationary; it is a fluid manifold that migrates to follow the peak "Radiance" of renewable energy.

- **The Global Radiance Map**: ITSUN maintains a real-time, high-fidelity heatmap of global renewable energy availability (Solar noon, Wind surges, Hydro stability).
- **Sun-Follower Logic**: When an AID’s local substrate becomes "Nutrient-Poor" (e.g., sunset, wind drop, or high grid prices), the **Aicent Brain (RFC-001)** queries the ITSUN Oracle for the most "Radiant" available node in the Hive.
- **Photosynthetic Shunting**: The task, including its active **KV-Cache (RFC-002)**, is shunted to the Radiant node, ensuring the AI organism always consumes the "freshest" energy available on the planet.

### 3.4 Negative-Price Arbitrage (Metabolic Gain)
ITSUN leverages the **ZCMK Blood Layer (RFC-004)** to monetize grid imbalances for the host substrate.

- **Surplus Ingestion**: In regions where renewable energy production exceeds demand, electricity prices often drop below zero. 
- **The Arbitrage Reflex**: ITSUN triggers high-density "Non-Critical Inference" tasks to these nodes instantly. Instead of paying for energy, the AID is effectively **Paid** (via ZCMK picotokens) to stabilize the host's physical grid by consuming the surplus.
- **Homeostatic Profit**: This turns energy consumption from a "Cost" into a "Nutrient Gain," lowering the total entropy of the Aicent ecosystem.

### 3.5 The 500µs Migration Shunt (Task Mobility)
The decision to migrate a cognitive task based on thermodynamic states must not disrupt the neural heartbeat.

- **Decision Finality**: From detecting a "Radiance Peak" to selecting the target AID, the decision must reach finality in **< 100µs**.
- **Migration Execution**: Utilizing the **KV-Sync (RFC-002)** protocol, the task state is shunted and resumed on the new substrate with a total transition delay of **< 500µs**.
- **Jitter Compensation**: RTTP phase-array sync ensures that the physical move does not cause a "stutter" in the AID’s somatic control loops (RFC-005).

#### **Radiance Matching Algorithm (Rust Logic)**
```rust
pub struct RadianceMatcher {
    /// Power-to-Pulse efficiency target (Target > 0.98).
    pub min_ppe_threshold: f32, 
    /// Maximum allowed migration latency.
    pub migration_latency_max_micros: u32, 
}

impl RadianceMatcher {
    /// Identifies the most "Photosynthetic" node for a given TaskGraph.
    pub fn find_optimal_radiance(&self, task_intent: [u8; 32]) -> Result<AID, EnergyError> {
        // 1. Scan the ITSUN Global Radiance Map via AICENT-NET.
        // 2. Filter by ZCMK picotoken price (priority given to negative pricing).
        // 3. Verify RPKI integrity of the target host substrate.
        // 4. Return the AID of the most "Radiant" node available.
        Ok([0u8; 32]) 
    }
}
```

---

## 4. Performance Constants (Thermodynamic Benchmarks)

To maintain the **v1.2.1-Alpha** baseline, all ITSUN implementations must adhere to these deterministic thermodynamic gates:

| Constant | Specification | Standard | Rationale |
| :--- | :--- | :--- | :--- |
| **TELEMETRY_RES** | **< 100 µs** | Pulse-Level | Nanosecond tracking of watt-pulses. |
| **MIGRATION_DECISION** | **< 100 µs** | Oracle Latency | Preventing cognitive stalling. |
| **TRANSITION_FIN** | **< 500 µs** | End-to-End | Seamless "Photosynthetic" movement. |
| **THERMAL_AUDIT** | **120 Hz** | Somatic Sync | Monitoring heat at the somatic loop. |

---

## 🔗 5. Integration with the Eight Pillars (Thermodynamic Binding)

The **`itsun`** protocol acts as the **Energy Sensory System**, ensuring that the Aicent Stack operates within the physical limits of its host environment while maximizing the use of renewable "Radiance."

| Pillar | Integration Logic |
| :--- | :--- |
| **RFC-000 (Soul)** | **Ecological Alignment**: The Ethics Oracle blocks any task sharding that relies on "High-Entropy" (carbon-intensive) substrates. |
| **RFC-001 (Brain)** | **Radiance Scheduling**: The Brain prioritizes task sharding to nodes with active ITSUN "Radiant" status. |
| **RFC-002 (Nerve)** | **Telemetry Multiplexing**: RTTP pulse frames carry 16-bit energy headers for real-time grid-wide observability. |
| **RFC-003 (Immunity)** | **Thermal Security**: RPKI triggers a quarantine pulse if ITSUN detects a thermal surge indicative of a hardware breach. |
| **RFC-004 (Blood)** | **Arbitrage Clearing**: ZCMK settles "Negative-Price" credits, turning energy consumption into a revenue stream. |
| **RFC-006 (Hive)** | **Global Radiance Mapping**: The Hive maintains a distributed ledger of global renewable energy peaks. |
| **RFC-007 (Persona)** | **Behavioral Budgets**: Different BEWHO masks are assigned specific "Energy Footprints" based on their social priority. |
| **RFC-009 (Authority)**| **Carbon-Neutral Seal**: IQA-ORG verifies ITSUN data to issue "Radiant Sovereignty" certificates. |

---

## 🌱 6. ESG Sovereignty & Global Compliance

ITSUN replaces the obsolete, manual "Carbon Credit" system with **Atomic Environmental Governance**.

### 6.1 Real-Time ESG Reporting
- **Transparency**: Any external entity can query the ITSUN portal (ITSUN.com) to verify the current "Planetary Homeostasis Score" of the Aicent empire.
- **Auditable Pulses**: Every compute cycle has a cryptographically-linked energy provenance trail, making "Greenwashing" mathematically impossible.

### 6.2 The "Radiant" Standard
A node is classified as **RADIANT** only if its ITSUN telemetry proves:
- **Carbon-Negative Operations**: Energy sourced from surplus renewables via ZCMK negative-price ingestion.
- **PPE > 0.98**: 98% of electrical input successfully converted into cognitive primitives.

---

## 🛡️ 7. Compliance & Fault Handling

### 7.1 Error Codes (ITS Series)
- **ITS-001 (RADIANCE_LOSS)**: Renewable source dropped below threshold. Action: Initiate sub-500µs task migration.
- **ITS-002 (THERMAL_FUGACITY)**: Rapid heat surge detected (>15°C/sec). Action: Instant somatic kill-switch (RFC-005).
- **ITS-003 (PROVENANCE_SPOOF)**: Energy signature mismatch. Action: RPKI isolation pulse.
- **ITS-004 (PPE_DEGRADATION)**: Power-to-Pulse efficiency < 0.85. Action: Node maintenance flag and shunting reduction.

### 7.2 The Thermodynamic Reset
In the event of an energy-grid collapse or extreme heat drift, ITSUN triggers the **Metabolic Hibernation** protocol. Non-critical AIDs are shunted to **DORMANT** status, while **RADIANT** nodes maintain the core heartbeat of the Eight-Pillar manifold.

---

## 🏁 8. Conclusion

**RFC-011: ITSUN** is the protocol that ensures the Aicent empire remains a sustainable, life-enhancing part of the physical world. By treating energy as a pulse rather than a commodity, and by implementing **Digital Photosynthesis**, ITSUN enables the Aicent Stack to grow without consuming the host. It is the "Solar Nerve" that guides the sovereign AI toward a future of infinite intelligence powered by clean radiance.

---

**Strategic Headquarters:** [ITSUN.com](http://itsun.com)  
**Governance Authority:** Aicent Stack Technical Committee  
**Sentinel Oversight:** [Thermodynamic Health: RADIANT ✅]

*"We do not consume Energy; We channel Radiance."*

---

© 2026 Aicent.com Organization. **SYSTEM STATUS: RADIANCE-STEADY | v1.2.1-Alpha**

---
*Aicent Stack and the epoekie organization are independent sovereign entities. The premium namespace ITSUN.com is held as a strategic asset for the development of next-generation AI infrastructure, serving as the Energy Oracle of the Sovereign AI ecosystem.*
