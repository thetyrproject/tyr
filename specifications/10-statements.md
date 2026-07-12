# 10. Statements

---

## 10.1 Overview

Statements define hardware behaviour.

Unlike software programming languages, statements in Tyr describe hardware relationships rather than sequential execution unless explicitly stated otherwise.

---

## 10.2 Statement Categories

The language defines the following statement categories.

- Assignment statements
- Conditional statements
- Flow blocks
- Event blocks
- Wait statements
- Assertion statements

---

## 10.3 Assignment

Assignment establishes a hardware connection between two compatible objects.

The assignment operator is:

```tyr
<-
```

Example:

```tyr
SUM <- A + B;
```

Assignments shall not imply sequential execution.

---

## 10.4 Conditional Statements

Conditional behaviour is expressed using:

```tyr
if

else
```

Example:

```tyr
if ENABLE {

    OUT <- IN;

}
else {

    OUT <- 0;

}
```

---

## 10.5 Match Statement

Multiple conditional alternatives may be expressed using:

```tyr
match
```

Example:

```tyr
match OPCODE {

    ...

}
```

---

## 10.6 Flow Blocks

A flow block describes continuously active hardware behaviour.

Example:

```tyr
flow {

    SUM <- A + B;

}
```

Statements within a flow block are evaluated according to the hardware execution model.

---

## 10.7 Event Blocks

Event blocks describe behaviour triggered by asynchronous events.

Event blocks are only valid within asynchronous systems.

---

## 10.8 Wait Statements

The `wait` statement suspends execution until a specified condition becomes true.

The exact semantics depend upon the selected execution model.

---

## 10.9 Assertions

Assertions verify hardware properties.

Assertion failures shall produce implementation diagnostics.

---

## 10.10 Statement Ordering

Unless explicitly defined by the language execution model, the textual order of independent statements shall not imply execution order.

Hardware descriptions are inherently concurrent.
