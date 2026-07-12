# Preface

**Tyr Language Specification**

**Draft Version 0.1**

---

## Purpose

This document defines the syntax, semantics, and behavioral rules of the Tyr Hardware Description Language.

Its purpose is to provide a complete and implementation-independent specification that enables compliant implementations of the language.

The specification serves as the normative definition of Tyr. Any compiler, interpreter, simulator, or tool claiming compliance with the Tyr language shall conform to the requirements defined by this document.

This specification does not describe a particular compiler implementation.

---

## Scope

This document specifies:

- lexical structure
- grammar
- language semantics
- type system
- module system
- concurrency model
- compilation model
- backend requirements

This document does not define:

- implementation algorithms
- compiler optimizations
- hardware synthesis techniques
- simulator architecture
- editor integrations

These remain implementation decisions.

---

## Normative Language

The following words are used throughout this specification with specific meanings.

| Word | Meaning |
|-------|---------|
| **shall** | mandatory requirement |
| **shall not** | prohibited behavior |
| **should** | recommended behavior |
| **should not** | discouraged behavior |
| **may** | optional behavior |
| **implementation-defined** | behavior that must be documented by an implementation |
| **unspecified** | behavior intentionally left unspecified |
| **undefined** | invalid program behavior |

These definitions are normative.

---

## Specification and Implementation

The Tyr language is defined by this specification.

Compiler implementations are expected to implement the language described herein.

Implementation behavior shall never redefine the language itself.

Whenever a discrepancy exists between this specification and an implementation, this specification shall be considered authoritative.

---

## Versioning

Language versions and compiler versions are independent.

The language specification defines the standard.

Compiler implementations provide one realization of that standard.

---

## Audience

This specification is intended for:

- compiler developers
- hardware engineers
- language designers
- simulator developers
- researchers
- educators
- students

No prior implementation knowledge is assumed.

---

## Acknowledgements

The Tyr Project is developed as an open-source community effort.

The authors gratefully acknowledge the contributions of every researcher, developer, educator, and community member who participates in the evolution of the language.

---

**One Language. Every Digital Architecture.**
