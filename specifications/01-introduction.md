# 1. Introduction

---

## 1.1 Overview

Tyr is a modern hardware description language designed for describing digital hardware systems.

Unlike traditional hardware description languages that evolved around specific implementation technologies, Tyr defines hardware through consistent language semantics while remaining independent of the physical medium used to implement a design.

The language supports synchronous and asynchronous digital systems through a unified programming model.

---

## 1.2 Objectives

The primary objectives of Tyr are:

- describe hardware rather than software
- provide a modern and expressive language
- remain independent of implementation technology
- support both binary and multi-valued logic
- enable deterministic hardware description
- encourage readable and maintainable designs

---

## 1.3 Design Approach

Tyr separates language definition from compiler implementation.

The language defines *what* a hardware description means.

Compiler implementations determine *how* that description is translated into target representations.

This separation allows multiple compliant implementations to exist while preserving language compatibility.

---

## 1.4 Supported Architectures

The language is designed to support a broad range of digital hardware architectures, including but not limited to:

- synchronous digital systems
- asynchronous digital systems
- binary logic systems
- balanced multi-valued logic systems
- FPGA architectures
- ASIC implementations
- emerging digital computing paradigms

Support for a target architecture is determined by the compiler backend rather than the language itself.

---

## 1.5 Language Philosophy

Tyr treats hardware as a collection of concurrent components rather than sequential instructions.

Every construct in the language represents hardware structure, hardware behavior, or relationships between hardware components.

The language does not attempt to emulate software programming models where such abstractions conflict with physical hardware.

---

## 1.6 Open Development

Tyr is developed through an open specification process.

Language evolution occurs through public discussion, Requests for Comments (RFCs), and community review.

Compiler implementations are expected to follow the published specification.

---

## 1.7 Future Evolution

Digital hardware continues to evolve.

The Tyr language is designed with sufficient flexibility to accommodate future hardware architectures while preserving backwards compatibility whenever practical.

Language evolution shall prioritize consistency and long-term stability over rapid feature growth.
