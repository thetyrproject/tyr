# 8. Types

---

## 8.1 Overview

Every object declared within a Tyr program shall possess a type.

Types define the representation, interpretation, and permitted operations of hardware objects.

The language distinguishes between primitive types and composite types.

---

## 8.2 Primitive Types

The Tyr language defines the following primitive types.

| Type | Description |
|------|-------------|
| `bit` | Binary logic value |
| `trit` | Balanced ternary logic value |
| `clock` | Clock signal |
| `event` | Event source |

---

## 8.3 Composite Types

Composite types are constructed from primitive types.

The language defines:

```
bus
array
```

Additional composite types may be introduced by future revisions.

---

## 8.4 Bit

The `bit` type represents a binary logic value.

Valid values are:

```
0
1
```

Implementations may provide additional simulation values.

Such values are implementation-defined.

---

## 8.5 Trit

The `trit` type represents a balanced ternary logic value.

The standard logical values are:

```
n
0
1
```

The interpretation of these values depends upon the selected hardware backend.

The language defines only their logical meaning.

---

## 8.6 Clock

The `clock` type represents a synchronization source.

Clock objects are meaningful only for synchronous hardware descriptions.

Use of clock objects in asynchronous systems shall produce a diagnostic.

---

## 8.7 Event

The `event` type represents an asynchronous triggering source.

Event objects are meaningful only within asynchronous hardware descriptions.

---

## 8.8 Bus

A bus represents an ordered collection of elements of identical type.

General form:

```tyr
bus<width,type>
```

Example:

```tyr
bus<32,bit>
```

```tyr
bus<27,trit>
```

---

## 8.9 Array

An array represents a fixed-size collection of objects.

General form:

```tyr
array<type,size>
```

Example:

```tyr
array<trit,256>
```

---

## 8.10 Type Compatibility

Operations shall only be performed upon compatible operand types.

Implicit conversions are intentionally limited.

Implementations shall diagnose incompatible type usage.

---

## 8.11 Future Types

Future language revisions may introduce additional primitive or composite types.

Existing type semantics shall remain unchanged whenever practical.
