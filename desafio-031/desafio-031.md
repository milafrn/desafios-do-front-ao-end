# :books: Desafio - 031

## Desafio 01 :pencil2:

---

### Desafio - 01.

> Apenas a função memoryCard do componente memoryCard pode ser acessível no escopo global. As demais funções (handleClick, activeMemoryCard, checksure) não devem ser acessíveis em escopo global. Deve ser usado IIFE (imediately Invoked Function Expression)

#### Dicas

- no momento que **`isolar`** irá **`expor`** apenas **`uma`** coisa para fora do **`IIFE`**.
- No momento que executar uma função como **expor uma coisa** para fora
- `Existe uma palavra reservada para isso`

- [x] [Desafio - 01](https://github.com/milafrn/jogo-da-memoria/commit/c90d94ef4a75a2310c2db97dacaf96ddf1d62e63)

---

### Desafio - 02.

> **Refletir** sobre o **`cards-wrapper`** se eu tenho que isolar tudo que está dentro dele. O que tem que ser feito?

> R: Não é necessário isolar tudo que está dentro do cards-wrapper, pois há necessidade de usa-lo no **`game`**. Se por acaso colocar IIFE no `cards-wrapper` só iria deixar o código mais complexo sem necessidade.

- Colocar o `qtdActiveMemoryCard` como váriavel global (isto sou eu que percebi que há necessidade).

- [x] [Desafio - 02](https://github.com/milafrn/jogo-da-memoria/commit/c90d94ef4a75a2310c2db97dacaf96ddf1d62e63)

---

### Desafio - 03.

> **Responder:** A funçao `checkSure` que está no componente `memoryCard` é responsabilidade do próprio componente ou é responsabilidade do `cards-wrapper`? onde a função `checkSure` Deve ficar?

#### Dica

- Lembrando que o **componente** ele tem que ser burro, ele deve apenas cuidar dele mesmo.

> R: A responsabilidade é do `cards-wrapper` por que o `memoryCard` é responsável apenas por ele mesmo e o `cards-wrapper` é o que envolve todos os `memoryCard` então a responsabilidade de checar o correto(`checkSure`) é do `cards-wrapper`.

- [x] [Desafio - 03](https://github.com/milafrn/jogo-da-memoria/commit/c90d94ef4a75a2310c2db97dacaf96ddf1d62e63)
