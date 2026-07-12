# 15. Memory Objects

---

## 15.1 Overview

Memory objects provide hardware storage for collections of values.

The Tyr language specifies observable memory behaviour while remaining independent of physical implementation.

---

## 15.2 Declaration

Memory objects are declared using the `memory` keyword.

The declaration specifies the stored type and implementation dimensions.

---

## 15.3 Organization

Memory organization is implementation-defined.

Possible implementations include:

- SRAM
- DRAM
- FPGA block memory
- distributed memory
- register arrays

The language does not distinguish between these implementations.

---

## 15.4 Addressing

Memory objects are indexed using integer expressions.

Address ranges shall remain within the declared bounds.

Out-of-range access shall produce a diagnostic whenever detectable.

---

## 15.5 Read Operations

Memory reads produce the value currently stored at the selected location.

Read latency is backend-dependent.

---

## 15.6 Write Operations

Memory writes modify the selected location.

The observable behaviour shall remain consistent across compliant implementations.

---

## 15.7 Initialization

Memory objects may be initialized during elaboration.

Initialization syntax is defined elsewhere in this specification.

---

## 15.8 Concurrent Access

Concurrent access to memory objects shall follow the execution model.

Whenever multiple writes target the same location simultaneously, behaviour is implementation-defined unless otherwise specified.

---

## 15.9 Backend Independence

The language defines logical memory behaviour.

Physical implementation remains the responsibility of the compiler backend.

Implementations shall preserve observable semantics regardless of target technology.
