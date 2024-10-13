# Decorator - Structural (Estrutural)

## Minha Opinião

Ao invés de criar subclasses para extender a característica de algum produto, podemos utilizar o design pattern Decorator, pois ele irá utilizar de objetos já criados para extender o código, sem a necessidade de alterá-lo, seguindo com rigor o princípio de aberto e fechado. Sobre sua implementação, achei uma das mais simples e fáceis de entender.

---

## Intenção

*Agregar responsabilidades adicionais a um objeto dinamicamente. Os Decorators fornecem uma alternativa flexível ao uso de subclasses para extensão de funcionalidades.*

---

## Sobre o Decorator

O Decorator é uma padrão de projeto usado para adicionar funcionalidades a objetos já criados, ou seja, sem a necessidade de alterar nenhum código. Isso faz com que este padrão aplique naturalmente o princípio do aberto/fechado (classes devem estar abertas para extensão, mas fechadas para modificação).

---

## Aplicabilidade

Use o padrão Decorator quando:

- você precisa adicionar funcionalidades em objetos sem quebrar ou alterar o código existente
- você quiser usar composição ao invés de herança
- você percebe que pode ocorrer uma explosão de subclasses em determinada estrutura

## Consequências

O que é bom ou ruim no Decorator:

**Bom:**
- Composição é melhor do que herança em grande maioria dos casos
- É fácil adicionar ou remover comportamento de objetos sem tocar em código já escrito ou testado (OCP)
- É possível decorar um objeto já decorado, adicionando ainda mais funcionalidades (camadas)

**Ruim:**
- Quanto mais decorators em camadas, mais complexo seu código se torna