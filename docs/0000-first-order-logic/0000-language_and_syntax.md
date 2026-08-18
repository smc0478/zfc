---
title: Language and Syntax
lang: en
en_url: /0000-first-order-logic/0000-language_and_syntax.html
ko_url: /0000-first-order-logic/0000-language_and_syntax_kr.html
---

# Language and Syntax

This section defines the symbols and the rules for well-formed formulas (wffs) needed for ZFC.

## Symbols

### Variables

There are countably many variables, such as $x_0,x_1,\ldots$, used to represent sets.

### Quantifier symbols

<table>
  <tr>
    <td>$\forall$</td>
    <td>Expresses that every object has a given property.<br>
        e.g. $\forall x(x=x)$</td>
  </tr>
  <tr>
    <td>$\exists$</td>
    <td>Expresses the existence of an object with a given property.<br>
        e.g. $\exists x(x=x)$</td>
  </tr>
</table>

### Logical connectives

<table>
  <tr>
    <td>$\neg$</td>
    <td>Logical negation (“not”).</td>
  </tr>
  <tr>
    <td>$\land$</td>
    <td>Logical conjunction (“and”).</td>
  </tr>
  <tr>
    <td>$\lor$</td>
    <td>Logical disjunction (“or”).</td>
  </tr>
</table>

### Parentheses

The symbols $($ and $)$ are used to indicate precedence.

### Equality symbol

The symbol $=$ denotes equality in the usual sense.

### Set-membership symbol

The expression $a \in b$ states that $a$ is an element of the set $b$.

## Recursive definition of well-formed formulas

Let $x$ and $y$ be metavariables for any variables. The following expressions are well-formed formulas; they are called **atomic formulas**.

- $x = y$
- $x \in y$

Let $\phi$ and $\psi$ be metavariables for any well-formed formulas. The following expressions are also well-formed formulas.

- $\neg \phi$
- $(\phi \lor \psi)$
- $(\phi \land \psi)$
- $\forall x\ \phi$
- $\exists x\ \phi$

Only expressions obtained by applying these rules finitely many times are well-formed formulas.
