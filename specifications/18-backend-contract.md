# 18. Backend Contract

---

## 18.1 Overview

Compiler backends translate Tyr hardware descriptions into implementation-specific representations.

Backends are responsible for preserving language semantics.

---

## 18.2 Backend Independence

The Tyr language shall remain independent of backend implementation.

Changing the compilation target shall not alter the logical meaning of a hardware description.

---

## 18.3 Semantic Preservation

Every compliant backend shall preserve:

- type correctness
- concurrency
- execution model
- hardware connectivity
- module hierarchy

---

## 18.4 Backend Responsibilities

Backends are responsible for:

- code generation
- target validation
- implementation diagnostics
- technology mapping

---

## 18.5 Implementation Limits

Backend limitations shall be documented.

Unsupported hardware features shall produce diagnostics.

---

## 18.6 Future Targets

This specification intentionally permits future backend targets.

Examples include:

- Verilog
- VHDL
- simulation environments
- FPGA toolchains
- ASIC toolchains

---

## 18.7 Compliance

Backend correctness shall be evaluated according to observable hardware behaviour rather than generated source code.
