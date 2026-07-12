# 13. Concurrency Model

---

## 13.1 Overview

Concurrency is the fundamental execution model of the Tyr language.

Unless explicitly specified otherwise, hardware described in Tyr shall operate concurrently.

Sequential interpretation shall never be inferred solely from textual ordering.

---

## 13.2 Concurrent Hardware

Hardware objects exist simultaneously.

Independent hardware operations shall be considered active concurrently.

Example:

```tyr
flow {

    A <- B;

    C <- D;

}
```

The above assignments represent concurrent hardware.

---

## 13.3 Sequential Behaviour

Sequential behaviour shall be expressed explicitly.

The language does not infer sequential execution from source code layout.

---

## 13.4 Independent Operations

Independent operations may execute simultaneously.

Compiler implementations may evaluate independent operations in any order that preserves observable hardware behaviour.

---

## 13.5 Dependency

Whenever one hardware operation depends upon another, the dependency shall be explicitly represented within the hardware description.

Dependencies are determined by data flow rather than source code order.

---

## 13.6 Combinational Behaviour

Combinational hardware responds continuously to changes in its inputs.

Combinational descriptions shall not introduce unintended storage.

---

## 13.7 Sequential Hardware

Sequential hardware retains state between evaluations.

Sequential hardware shall be explicitly defined through clocks or events.

---

## 13.8 Cyclic Dependencies

Combinational cycles are prohibited unless explicitly supported by the selected backend.

Implementations shall diagnose illegal combinational feedback.

---

## 13.9 Determinism

Equivalent hardware descriptions shall produce equivalent concurrent behaviour.

Compiler optimizations shall not alter observable semantics.
