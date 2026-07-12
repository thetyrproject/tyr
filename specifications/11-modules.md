# 11. Modules

---

## 11.1 Overview

A module is the fundamental design unit of the Tyr language.

Modules describe reusable hardware components.

Every Tyr hardware design shall consist of one or more modules.

---

## 11.2 Module Declaration

A module declaration begins with the `module` keyword and terminates with the `end` keyword.

General form:

```tyr
module Identifier

...

end
```

---

## 11.3 Module Name

Every module shall possess a unique identifier within its enclosing namespace.

Module names are case-sensitive.

---

## 11.4 Interface

Modules communicate exclusively through declared interfaces.

Interfaces consist of:

- input
- output
- inout

Interface declarations shall appear before behavioural descriptions.

---

## 11.5 Internal Objects

Modules may contain:

- signals
- registers
- memories
- constants
- buses
- arrays
- subordinate modules

---

## 11.6 Behaviour

Hardware behaviour shall be described using one or more behavioural blocks.

The language currently defines:

- flow blocks
- event blocks

Additional block types may be introduced by future revisions.

---

## 11.7 Module Instantiation

Modules may instantiate other modules using the `use` keyword.

Example:

```tyr
use HalfAdder HA0;
```

Module instantiation creates a hardware instance.

---

## 11.8 Hierarchy

Modules may be composed hierarchically.

Recursive module instantiation is prohibited.

---

## 11.9 Visibility

Objects declared within a module are visible only within that module unless explicitly exported through its interface.

---

## 11.10 Translation Unit

A Tyr source file may contain multiple module declarations.

The translation unit consists of the complete source file after compiler directives have been processed.

---

## 11.11 Design Philosophy

Modules represent hardware structure rather than software abstraction.

Module decomposition should improve readability, reuse, verification, and maintainability without altering hardware semantics.
