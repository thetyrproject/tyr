# 9. Expressions

---

## 9.1 Overview

Expressions describe the computation of values within a hardware design.

An expression shall evaluate to a value of a well-defined type.

Expressions shall not create or destroy hardware.

Instead, expressions describe the logical relationship between hardware objects.

---

## 9.2 Expression Categories

The Tyr language defines the following expression categories.

- Primary expressions
- Unary expressions
- Binary expressions
- Conditional expressions
- Function expressions (future)

---

## 9.3 Primary Expressions

Primary expressions include:

- identifiers
- literals
- parenthesized expressions

Example:

```tyr
A

1

n

(A + B)
```

---

## 9.4 Unary Expressions

Unary operators operate upon a single operand.

Examples include:

```tyr
tnot A

!READY

-A
```

---

## 9.5 Binary Expressions

Binary operators operate upon two operands.

Examples:

```tyr
A + B

A tand B

X * Y

LEFT == RIGHT
```

Operands shall possess compatible types.

---

## 9.6 Parenthesized Expressions

Parentheses explicitly define evaluation order.

Example:

```tyr
(A + B) * C
```

Nested parentheses are permitted.

---

## 9.7 Type Rules

Every expression possesses exactly one type.

The resulting type shall be determined according to the language type rules.

Implicit type conversion is not performed.

Implementations shall diagnose incompatible operand types.

---

## 9.8 Constant Expressions

An expression composed entirely of constant values may be evaluated during compilation.

Compile-time evaluation shall not alter observable language semantics.

---

## 9.9 Side Effects

Expressions shall not possess observable side effects.

Hardware state changes shall occur only through statements defined by this specification.

---

## 9.10 Future Extensions

Future language revisions may introduce additional expression forms without altering the semantics defined herein.
