# 5. Tokens

---

## 5.1 Overview

The lexical analyzer converts a sequence of source characters into a sequence of tokens.

Tokens form the smallest meaningful units of the language.

Every Tyr program is interpreted as a sequence of tokens.

---

## 5.2 Token Categories

The Tyr language defines the following token categories.

| Category | Description |
|-----------|-------------|
| Keywords | Reserved language words |
| Identifiers | User-defined names |
| Literals | Constant values |
| Operators | Arithmetic and logical operators |
| Punctuation | Delimiters and separators |
| Compiler Directives | Compilation instructions |

---

## 5.3 Keywords

Keywords are reserved identifiers with predefined language meaning.

Keywords shall not be used as identifiers.

The complete keyword list is defined in Chapter 6.

---

## 5.4 Identifiers

Identifiers name language entities including:

- modules
- signals
- registers
- memories
- constants
- user-defined types

Identifier syntax is defined by the lexical grammar.

---

## 5.5 Literals

Literals represent constant values.

The language defines literals for:

- binary values
- balanced ternary values
- numeric constants
- strings
- arrays (future)

Literal syntax is specified in later chapters.

---

## 5.6 Operators

Operators define relationships between operands.

Operator categories include:

- arithmetic
- logical
- comparison
- assignment
- bitwise
- ternary logic

Operator precedence is defined separately.

---

## 5.7 Punctuation

Punctuation tokens delimit language constructs.

Examples include:

```
(
)

{

}

[

]

,

;

:
```

Additional punctuation symbols may be defined by future revisions.

---

## 5.8 Compiler Directives

Compiler directives begin with the `#` character.

Compiler directives influence compilation behavior.

Compiler directives are processed before semantic analysis.

Examples include:

```tyr
#system async

#target verilog
```

---

## 5.9 Longest Match Rule

When multiple token interpretations are possible, lexical analysis shall select the longest valid token.

---

## 5.10 Invalid Tokens

Character sequences that do not form valid tokens shall produce a lexical diagnostic.

Processing beyond the diagnostic is implementation-defined.
