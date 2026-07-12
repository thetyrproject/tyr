# 6. Keywords

---

## 6.1 Overview

Keywords are reserved identifiers that possess predefined meaning within the Tyr language.

Keywords form part of the language grammar and shall not be redefined by user programs.

An implementation shall recognize every keyword defined by this specification.

---

## 6.2 Reserved Keywords

The following keywords are reserved for use by the Tyr language.

### Module Declaration

```
module
end
use
```

---

### Interface Declaration

```
input
output
inout
```

---

### Data Objects

```
signal
register
memory
const
```

---

### Primitive Types

```
bit
trit
bus
array
clock
event
```

---

### Behaviour

```
flow
if
else
match
default
return
```

---

### Verification

```
assert
assume
cover
```

---

### Timing

```
wait
after
delay
```

---

### Ternary Operators

```
tand
tor
txor
tnot
```

---

## 6.3 Future Reserved Keywords

The following identifiers are reserved for future language evolution.

```
enum
struct
union
interface
package
namespace
generic
```

Programs shall not use future reserved keywords as identifiers.

---

## 6.4 Keyword Restrictions

Keywords shall not be used as:

- identifiers
- module names
- signal names
- register names
- constants
- user-defined types

Attempting to redefine a keyword shall produce a diagnostic.

---

## 6.5 Case Sensitivity

Keywords are case-sensitive.

The following are distinct:

```
module
Module
MODULE
```

Only the lowercase spelling is recognized as a keyword.

---

## 6.6 Language Evolution

Future versions of Tyr may introduce additional reserved keywords.

Language revisions should minimize disruption to existing programs whenever practical.
