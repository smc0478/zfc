---
title: 언어와 문법
lang: ko
en_url: /0000-first-order-logic/0000-language_and_syntax.html
ko_url: /0000-first-order-logic/0000-language_and_syntax_kr.html
---

# Language and Syntax
ZFC에 필요한 기호와 well-formed fomula (wff) 규칙을 정의한다.

## 기호(Symbols)
### 변수(Variable)
$x_0, x_1, \ldots$ 등의 가산 무한개의 변수를 사용한다.
### 양화사(quantifier symbols)
<table>
  <tr>
    <td>$\forall$</td>
    <td>모든 대상에 대하여 주어진 성질이 성립함. <br>
        예) $\forall x(x = x)$</td>
  </tr>
  <tr>
    <td>$\exists$</td>
    <td>주어진 성질을 만족하는 대상이 존재함. <br> 
        예) $\exists x(x=x)$</td>
  </tr>
</table>

### 논리 연결사(logical connectives)

<table>
  <tr>
    <td>$\neg$</td>
    <td>not 연산을 한다.</td>
  </tr>
  <tr>
    <td>$\land$</td>
    <td>and 연산을 한다.</td>
  </tr>
  <tr>
    <td>$\lor$</td>
    <td>or 연산을 한다.</td>
  </tr>
</table>

### 괄호(parentheses)
(,): 식의 구조와 연산의 우선순위를 나타내기 위해 사용한다.
### 등호(equality symbol)
=: 일반적으로 생각하는 등호의 기능이다.
### 원소 관계 기호(the set membership symbol)
$\in$: $a \in b$ 이면 원소 a는 집합 b의 원소다.

## Well-formed formula를 위한 재귀적인 정의
$x,y$를 변수에 대한 임의의 메타 변수라고 하자. 다음은 wff고 이는 **원자 논리식**이다.
- $x = y$
- $x \in y$

$\phi, \psi$를 wff에 대한 임의의 메타 변수라고 하자. 다음은 wff다.
- $\neg \phi$
- $(\phi \lor \psi)$
- $(\phi \land \psi)$
- $\forall x\ \phi$
- $\exists x\ \phi$

위 규칙들을 유한 번 적용하여 얻어지는 식만을 wff라고 한다.
