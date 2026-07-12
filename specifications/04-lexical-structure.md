# 4. Lexical Structure

---

## 4.1 Source Files

A Tyr source file shall consist of a sequence of Unicode characters encoded using UTF-8.

Source files typically use the `.tyr` file extension.

---

## 4.2 Character Set

The Tyr language uses the Unicode character set.

Language keywords and identifiers are currently restricted to the ASCII subset.

Future revisions may expand identifier support.

---

## 4.3 Whitespace

Whitespace separates lexical tokens.

The following characters are considered whitespace:

- Space (`U+0020`)
- Horizontal Tab (`U+0009`)
- Line Feed (`U+000A`)
- Carriage Return (`U+000D`)

Multiple whitespace characters are treated as a single separator unless otherwise specified.

---

## 4.4 Newlines

Newlines have no semantic meaning except where required by compiler directives.

Programs may freely span multiple lines.

---

## 4.5 Case Sensitivity

The Tyr language is case-sensitive.

The following identifiers are distinct:

```
signal
Signal
SIGNAL
```

---

## 4.6 Comments

Two forms of comments are supported.

Single-line comments begin with:

```tyr
//
```

and continue until the end of the current line.

Multi-line comments begin with:

```tyr
/*
```

and terminate with:

```tyr
*/
```

Nested multi-line comments are not permitted.

---

## 4.7 Line Continuation

Explicit line continuation characters are not required.

Language grammar determines whether a declaration continues onto subsequent lines.

---

## 4.8 Source Encoding

Implementations shall accept UTF-8 encoded source files.

Behavior for other encodings is implementation-defined.

---

## 4.9 Source File Independence

The interpretation of a source file shall not depend upon platform-specific newline conventions or file system characteristics.

Compliant implementations shall treat equivalent source files identically regardless of operating system.
