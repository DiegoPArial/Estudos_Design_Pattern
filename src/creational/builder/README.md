# Builder - Creational (Criação)

## Minha Opinião

O que entendi sobre o design pattern "builder" foi que ele só será utilizado quando a criação de um objeto se tornar complexo, seja ele por objetos compostos de vários outros objetos, construtores ou algoritmos de criação complexos. Obtive dificuldades em entender todo o processo, mas conforme eu utilizar em implementações creio que me acostume e entenda melhor.

## Intenção

*Separar a construção de um objeto complexo da sua representação de modo que o mesmo processo de construção possa criar diferentes representações.*

---

## Destilando a intenção

A intenção acima significa que:

* O padrão sugere a separação do código que cria e o código que usa o objeto
* Trata da criação de objetos complexos (complexos de verdade), como:
  - Objetos com construtores muito complexos
  - Objetos compostos de vários objetos (composite)
  - Objetos com algoritmo de criação complexo

Além disso, o padrão também:

- Permite a criação de um objeto em etapas
- Permite method chaining (encadeamento de métodos)
- Permite que o objeto final varie em dados e tipo

---

## Aplicabilidade

Use o Builder quando:

- Use o Builder quando a criação do objeto se torna complexa
- Use o Builder quando quiser que o código seja capaz de gerar diferentes representações do mesmo objeto

## Consequências

O que é bom ou ruim no Builder:

**Bom:**
- Separa criação de utilização de objetos
- O cliente não precisa criar objetos diretamente
- O mesmo código pode construir objetos diferentes
- Ajuda na aplicação dos princípios SRP e OCP

**Ruim:**

- O código final pode se tornar muito complexo
