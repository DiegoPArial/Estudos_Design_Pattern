# Observer - Behavioural (Comportamental)

## Minha Opinião

Achei a implementação complexa, mas é fácil de entender sua aplicabilidade, pois será utilizado apenas quando será necessário notificar vários objetos sobre a mudança de outro. Ele pode ser utilizado em diversos tipos de sistemas.

---

## Intenção

*Define uma dependência um para muitos entre objetos, de modo que, quando um objeto muda de estado, todos os seus dependentes são automaticamente notificados e atualizados.*

--=

## Aplicabilidade

Use o Observer quando:

- você precisa notificar vários objetos sobre a mudança de estado de outro(s) objeto(s) 

## Consequências

O que é bom ou ruim no Observer:

**Bom:**
- Usa o SRP e OCP
- Facilita a comunicação entre objetos em tempo de execução

**Ruim:**
- Pode ser complexo ou impossível manter a ordem em que as notificações são enviadas