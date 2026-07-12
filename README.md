# Tyr

<div align="center">

<img src="https://raw.githubusercontent.com/thetyrproject/branding/main/tyr-logo-black.png" alt="Tyr Logo" width="180"/>

### One Language. Every Digital Architecture.

*A modern hardware description language for synchronous, asynchronous, binary, and multi-valued digital systems.*

</div>

---

## Overview

Tyr is an open-source hardware description language designed for modern digital hardware development.

Unlike traditional hardware description languages that evolved around a specific implementation technology, Tyr is designed around hardware semantics. Whether describing synchronous digital systems, asynchronous logic, binary architectures, balanced-ternary systems, or future computing paradigms, the language remains consistent while compiler backends adapt to the target platform.

The Tyr repository contains the **official language specification**.

The reference compiler is developed separately in the **tyrc** repository.

---

## Project Goals

- A modern hardware description language
- Technology-independent language semantics
- Native support for synchronous and asynchronous hardware
- First-class support for binary and multi-valued logic
- Open language specification
- Community-driven evolution through RFCs

---

## Repository Layout

```
docs/
├── specification/
├── examples/
└── decisions/
```

| Directory | Description |
|------------|-------------|
| `specification` | Official language specification |
| `examples` | Reference language examples |
| `decisions` | Historical design decisions |

---

## Current Status

🚧 **Draft Specification**

The language is currently under active design.

No part of the specification should be considered stable until Version 1.0.

---

## Related Repositories

| Repository | Purpose |
|------------|---------|
| `tyrc` | Reference compiler |
| `tyr-rfcs` | Language evolution proposals |
| `tyr-book` | Official documentation |
| `branding` | Official branding assets |
| `governance` | Project governance |

---

## Contributing

We welcome contributions from:

- Hardware engineers
- Compiler developers
- Researchers
- Students
- Open-source contributors

Please read **CONTRIBUTING.md** before opening an issue or submitting a pull request.

---

## License

Licensed under the Apache License, Version 2.0.

---

<div align="center">

**One Language. Every Digital Architecture.**

</div>
