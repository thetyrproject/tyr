# Appendix A — Formal Grammar

This appendix presents the formal grammar of the Tyr language.

The grammar is informative.

The normative language definition is provided by the preceding chapters.

---

## Lexical Elements

```
identifier
integer
literal
keyword
operator
punctuation
```

---

## Module

```ebnf
translation-unit

    ::= directive*
        module+

module

    ::= "module"
        identifier
        module-body
        "end"
```

---

## Interfaces

```ebnf
interface

    ::= input-declaration
     | output-declaration
     | inout-declaration
```

---

## Statements

```ebnf
statement

    ::= assignment
     | if-statement
     | flow-block
     | event-block
     | wait-statement
```

---

## Expressions

```ebnf
expression

    ::= primary
     | unary-expression
     | binary-expression
```

The complete grammar will evolve with future language revisions.
