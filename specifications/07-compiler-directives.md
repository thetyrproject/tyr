# 7. Compiler Directives

---

## 7.1 Overview

Compiler directives provide instructions to the implementation that influence compilation behaviour.

Compiler directives are evaluated before lexical and semantic analysis.

Compiler directives are not part of the executable hardware description.

---

## 7.2 Syntax

A compiler directive begins with the `#` character.

General form:

```tyr
#directive arguments
```

Whitespace between the directive name and its arguments is optional unless otherwise specified.

---

## 7.3 System Model

The `#system` directive selects the execution model for the current translation unit.

Examples:

```tyr
#system sync
```

```tyr
#system async
```

Exactly one system model shall be specified for every translation unit.

If omitted, compiler behaviour is implementation-defined.

---

## 7.4 Backend Target

The `#target` directive specifies the intended backend.

Example:

```tyr
#target verilog
```

Future targets may include:

```
vhdl
tpa1
simulation
```

Backends shall not alter language semantics.

---

## 7.5 Language Version

The `#version` directive specifies the language version expected by the source file.

Example:

```tyr
#version 0.1
```

Implementations shall diagnose unsupported language versions.

---

## 7.6 Import Directives

The `#import` directive imports external language modules.

Example:

```tyr
#import math
```

The semantics of module resolution are implementation-defined.

---

## 7.7 Ordering

Compiler directives should appear before the first module declaration.

Implementations may reject directives appearing elsewhere.

---

## 7.8 Unknown Directives

Unknown compiler directives shall produce a diagnostic.

---

## 7.9 Duplicate Directives

If multiple directives define conflicting compilation behaviour, the implementation shall produce a diagnostic.

---

## 7.10 Future Extensions

Additional compiler directives may be introduced in future language revisions.

Compiler directives beginning with implementation-specific prefixes are implementation-defined.
