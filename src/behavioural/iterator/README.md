# Iterator - Behavioural (Comportamental)

## Minha Opinião

Este design pattern é utilizado com estrutura de dados, ou seja, convém criar um iterador em uma pilha ou uma fila, pois além de separar as responsabilidades, deixa uma porta aberta caso seja necessário criar novos iteradores. Achei o código um pouco complexo.

---

## Intenção

*Fornece uma maneira de acessar sequencialmente os elementos de um objeto agregado sem expor sua representação subjacente.*

---

## Aplicabilidade

Use o Iterator quando:

- você precisa remover a complexidade de travessia de dentro da coleção principal. Isso permite que sua coleção foque apenas em armazenar dados de maneira eficiente
- sua coleção pode ter vários modos de travessia, como crescente, decrescente,  pelo menor número de saltos, pulando de dois em dois, ou como preferir
- você quer disponibilizar protocolos de travessia para diferentes tipos coleções 

## Consequências

O que é bom ou ruim no Iterator:

**Bom:**
- É possível pausar a travessia e continuar posteriormente
- É possível atravessar várias vezes a mesma coleção em paralelo usando outro objeto iterador
- É fácil adicionar novos objetos iteradores com algoritmos de travessia completamente diferentes
- Não polui o código do objeto principal com vários métodos e algoritmos de travessia diferentes


**Ruim:**
- Este padrão só é útil se sua coleção realmente precisar de uma travessia complexa. Do contrário é apenas complexidade a mais.
