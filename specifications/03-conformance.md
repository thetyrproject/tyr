# 3. Conformance

---

## 3.1 Purpose

This chapter defines the requirements for implementations claiming conformance with the Tyr language specification.

The purpose of conformance is to ensure that Tyr programs have a consistent meaning across different implementations.

---

## 3.2 Conforming Implementations

A conforming implementation shall:

- implement the language semantics defined by this specification;
- correctly recognize all valid language constructs;
- reject invalid programs with appropriate diagnostics;
- document all implementation-defined behavior;
- report the supported language version.

Conformance applies independently of the target backend.

---

## 3.3 Language Version

Every implementation shall report the language specification version against which it is compliant.

Example:

```
Tyr Language Specification 0.1
```

Compiler version numbers are independent of language specification versions.

---

## 3.4 Diagnostics

When a program violates this specification, a conforming implementation shall produce at least one diagnostic.

The wording and presentation of diagnostics are implementation-defined.

---

## 3.5 Extensions

Implementations may provide language extensions.

Extensions shall not alter the meaning of valid Tyr programs.

Whenever extensions are enabled, the implementation should provide a mechanism for disabling them to ensure specification compliance.

---

## 3.6 Implementation-Defined Behaviour

Whenever this specification describes behavior as implementation-defined, implementations shall document the chosen behavior.

Examples include:

- backend-specific optimization decisions;
- supported synthesis targets;
- implementation limits.

---

## 3.7 Unspecified Behaviour

Certain aspects of the language are intentionally left unspecified.

Different implementations may choose different behavior in these cases without documentation requirements.

Programs shall not depend upon unspecified behavior.

---

## 3.8 Undefined Behaviour

Programs that violate language rules exhibit undefined behavior.

Implementations are not required to diagnose every instance of undefined behavior.

The results of undefined behavior are not constrained by this specification.

---

## 3.9 Future Compatibility

Implementations should avoid introducing extensions that conflict with potential future versions of the Tyr language.

Language evolution shall remain the responsibility of the Tyr specification.
