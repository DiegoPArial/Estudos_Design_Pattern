# Chain Of Responsibility - Behavioural (Comportamental)

## Minha Opinião

É um design pattern simples de entender, pois sempre será envolvido um escalonamento em que o próximo tem a capacidade de resolver o que o anterior não conseguiu, sua implementação dependendo de como for realizada, pode ser complexa.

---

## Intenção

*Evitar o acoplamento do remetente de uma solicitação ao seu destinatário, dando a mais de um objeto a chance de tratar a solicitação. Encadeia os objetos receptores e passa a solicitação ao longo da cadeia até que um objeto a trate*

---

## Aplicabilidade

Use o Chain Of Responsibility quando:

- seu sistema precisa processar uma requisição em várias etapas diferentes e você não quer criar uma ordem rígida para o processamento. O chain of responsibility permite que você altere a ordem dos objetos na cadeia facilmente (mesmo assim, mantendo uma ordem específica)
- você quer aplicar o princípio da responsabilidade única para tratamento de dados da requisição. Cada objeto fica responsável por tratar apenas a parte que lhe couber
- você quer permitir que os objetos responsáveis pelo tratamento de requisição possam variar em tempo de execução

## Consequências

O que é bom ou ruim no Chain Of Responsibility:

**Bom:**
- Aplica o princípio da responsabilidade única (SRP)
- Aplica o princípio do aberto e fechado (OCP)
- Permite que você altere a cadeia de objetos e a ordem das chamadas facilmente

**Ruim:**
- é comum uma requisição passar por toda a cadeia e não ser tratada