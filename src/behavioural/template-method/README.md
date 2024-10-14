# Template Method - Behavioural (Comportamental)

## Minha Opinião

Pelo o que entendi sobre este design pattern baseado no exemplo em código, ele pode enviar a definição de alguns passos da classe para as subclasses, sem mudar a estrutura. Sua implementação achei complexa e um pouco confusa.  

---

## Intenção

*Define o esqueleto de um algoritmo em uma operação, postergando a definição de alguns passos para subclasses. O template method permite que as subclasses redefinam certos passos de um algoritmo sem mudar sua estrutura*

---

## Aplicabilidade

Use o Template Method quando:

- você precisa de variações de um mesmo algoritmo sem mudar a ordem de execução dos métodos
- você percebe que está usando herança para alterar apenas pequenos trechos de código de um algoritmo

## Consequências

O que é bom ou ruim no Template Method:

**Bom:**
- Evita duplicação de código
- Permite fácil alteração de algoritmos
- Aplica o OCP e SRP

**Ruim:**
- Em alguns casos pode violar o LSP ao alterar o comportamento de métodos nas subclasses