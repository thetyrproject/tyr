# 2. Language Philosophy

The design of Tyr is guided by a small set of fundamental principles.

These principles define the long-term direction of the language and serve as the basis for evaluating future language features.

Whenever possible, language evolution should strengthen these principles rather than weaken them.

---

## 2.1 Hardware First

Tyr is a hardware description language.

Every language construct shall correspond to a meaningful hardware concept.

Language features that exist solely to imitate software programming languages should be avoided.

---

## 2.2 Technology Independence

The language shall remain independent of implementation technology.

A hardware description written in Tyr should preserve its meaning regardless of whether the target implementation is synchronous, asynchronous, binary, multi-valued, FPGA-based, ASIC-based, or another compliant digital architecture.

Implementation technology is the responsibility of the compiler backend.

---

## 2.3 Concurrency by Default

Digital hardware operates concurrently.

Concurrency is therefore the default execution model of Tyr.

Sequential behavior shall be expressed explicitly rather than implicitly assumed.

---

## 2.4 Deterministic Semantics

Equivalent Tyr programs shall produce equivalent hardware descriptions.

The language shall avoid context-dependent behavior, hidden state, or ambiguous interpretation.

Deterministic semantics are essential for reproducible hardware design.

---

## 2.5 Simplicity

Language complexity should only increase when a measurable improvement in expressiveness, correctness, or usability is achieved.

Simple language constructs are preferred over multiple overlapping mechanisms.

---

## 2.6 Orthogonality

Language features should interact predictably.

Whenever possible, similar constructs should follow similar rules.

Special cases should be minimized.

---

## 2.7 Explicitness

Hardware behavior should be visible within the source code.

Implicit hardware generation should be avoided.

Design intent should be understandable through inspection of the source.

---

## 2.8 Specification Before Implementation

The language specification defines Tyr.

Compiler implementations shall follow the specification.

Compiler limitations shall not redefine language semantics.

---

## 2.9 Stability

The language should evolve conservatively.

Backward compatibility should be preserved whenever practical.

Breaking language changes should be considered exceptional.

---

## 2.10 Open Evolution

The Tyr language is developed through open discussion.

Significant language changes should be proposed through the RFC process before becoming part of the specification.

Community participation is encouraged throughout the design process.

---

## 2.11 The Tyr Philosophy

The Tyr Project seeks to provide a language that remains relevant as digital hardware evolves.

Rather than defining hardware in terms of today's implementation technologies, Tyr defines hardware through enduring concepts that transcend any particular architecture.

The language should evolve with computing while remaining simple, predictable, and technically rigorous.

---

> **One Language. Every Digital Architecture.**
