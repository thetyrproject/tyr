# Contributing to Tyr

First of all, thank you for your interest in contributing to the Tyr Project.

Tyr is an open, community-driven language specification. Every contribution—whether documentation, examples, language proposals, or compiler development—helps improve the project.

---

# Before Contributing

Please read:

- The language specification
- The project governance documents
- Existing issues
- Existing RFCs

Many questions have already been discussed.

---

# Reporting Issues

When opening an issue, please include:

- Clear description
- Expected behaviour
- Current behaviour
- Relevant examples
- Specification references (if applicable)

---

# Pull Requests

Every pull request should focus on a single logical change.

Large changes should first be discussed through an Issue or RFC.

---

# Language Changes

Language features are not added directly.

The process is:

Issue

↓

Discussion

↓

RFC

↓

Community Feedback

↓

Maintainer Approval

↓

Specification Update

↓

Compiler Implementation

The specification always comes before implementation.

---

# Documentation

Documentation improvements are always welcome.

Please keep documentation:

- technically accurate
- concise
- implementation-independent
- grammatically correct

---

# Code Style

Compiler development follows the Rust style guide.

Formatting:

```
cargo fmt
```

Linting:

```
cargo clippy
```

All code should compile without warnings.

---

# Commit Messages

Use clear commit messages.

Examples:

```
lexer: add numeric literal tokenizer

spec: define module declaration grammar

parser: improve diagnostic recovery

docs: clarify signal lifetime rules
```

Avoid generic commit messages such as:

```
update

fix

changes

misc
```

---

# Branches

The `main` branch is protected.

All contributions should be submitted through Pull Requests.

---

# Respect the Specification

The Tyr Project follows one important principle:

> **The compiler implements the specification.**

The specification does not change to match compiler behaviour.

---

# Be Respectful

We welcome contributors from every background.

Disagree with ideas.

Never attack people.

Constructive discussion produces better language design.

---

Thank you for helping build Tyr.

**One Language. Every Digital Architecture.**
