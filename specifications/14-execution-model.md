# 14. Execution Model

---

## 14.1 Overview

The execution model defines how hardware descriptions respond to changes in hardware state.

The execution model is selected through the `#system` compiler directive.

---

## 14.2 Supported Models

The language defines two execution models.

```
sync

async
```

Future revisions may introduce additional execution models.

---

## 14.3 Synchronous Model

Under the synchronous model, state changes occur relative to one or more clock objects.

Clock events define synchronization boundaries.

Combinational hardware remains continuously active.

---

## 14.4 Asynchronous Model

Under the asynchronous model, state changes occur in response to explicitly defined events.

No global clock is assumed.

Hardware reacts whenever triggering conditions become satisfied.

---

## 14.5 Flow Blocks

Flow blocks represent continuously active hardware.

Flow blocks are valid under both execution models.

---

## 14.6 Event Blocks

Event blocks are valid only within asynchronous systems.

Use of event blocks within synchronous systems shall produce a diagnostic.

---

## 14.7 Clock Objects

Clock objects are valid only within synchronous systems.

Use of clock objects within asynchronous systems shall produce a diagnostic.

---

## 14.8 Wait Statements

The semantics of the `wait` statement depend upon the selected execution model.

Implementations shall preserve the observable behaviour defined by this specification.

---

## 14.9 Mixed Behaviour

A single translation unit shall define exactly one execution model.

Mixing synchronous and asynchronous execution models within a translation unit is prohibited.

Future revisions may define controlled interoperability mechanisms.
