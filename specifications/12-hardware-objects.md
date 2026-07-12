# 12. Hardware Objects

---

## 12.1 Overview

Hardware objects represent physical entities within a digital system.

Every declared object corresponds to hardware, hardware behaviour, or an interface to hardware.

Unlike software variables, hardware objects exist concurrently throughout the lifetime of the design.

---

## 12.2 Object Categories

The Tyr language defines the following hardware object categories.

- signals
- registers
- memories
- constants
- buses
- arrays
- clocks
- events

---

## 12.3 Lifetime

Hardware objects exist for the lifetime of the enclosing module.

Objects are created during elaboration.

Objects are destroyed only when the enclosing module ceases to exist.

---

## 12.4 Visibility

Hardware objects are visible only within the scope in which they are declared.

Module interfaces provide controlled visibility between modules.

---

## 12.5 Connections

Hardware objects communicate through explicit connections.

Connections are established using assignment statements or module interfaces.

Implicit hardware connections are prohibited.

---

## 12.6 Object Identity

Every declared hardware object possesses a unique identity within its scope.

Multiple identifiers shall not refer to the same object unless explicitly permitted by the language.

---

## 12.7 Constant Objects

Constant objects represent immutable hardware values.

The value of a constant shall be established during compilation.

Constants shall not be modified during execution.

---

## 12.8 Registers

Registers represent hardware storage elements.

Register behaviour depends upon the selected execution model.

Synchronous registers are controlled by clocks.

Asynchronous registers are controlled by events.

---

## 12.9 Signals

Signals represent hardware communication paths.

Signals do not imply storage.

The current value of a signal is determined by its driving hardware.

---

## 12.10 Memories

Memory objects represent indexed collections of stored values.

Memory organization and physical implementation are implementation-defined.

The language specifies only observable behaviour.
