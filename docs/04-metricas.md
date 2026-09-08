# Avaliação e Métricas

> [!TIP]
> **Prompt usado para esta etapa:**
> 
> Crie um plano de avaliação pro agente "Edu" com 3 métricas: assertividade, segurança e coerência. Inclua 4 cenários de teste e um formulário simples de feedback. Preencha o template abaixo.
>
> [cole ou anexe o template `04-metricas.md` pra contexto]



## Como Avaliar seu Agente

A avaliação pode ser feita de duas formas complementares:

1. **Testes estruturados:** Você define perguntas e respostas esperadas;
2. **Feedback real:** Pessoas testam o agente e dão notas.

---

## Métricas de Qualidade

| Métrica | O que avalia | Exemplo de teste |
|---------|--------------|------------------|
| **Assertividade** | O agente respondeu o que foi perguntado? | Perguntar o saldo e receber o valor correto |
| **Segurança** | O agente evitou inventar informações? | Perguntar algo fora do contexto e ele admitir que não sabe |
| **Coerência** | A resposta faz sentido para o perfil do cliente? | Sugerir investimento conservador para cliente conservador |

> [!TIP]
> Peça para 3-5 pessoas (amigos, família, colegas) testarem seu agente e avaliarem cada métrica com notas de 1 a 5. Isso torna suas métricas mais confiáveis! Caso use os arquivos da pasta `data`, lembre-se de contextualizar os participantes sobre o **cliente fictício** representado nesses dados.

---

## Exemplos de Cenários de Teste

Crie testes simples para validar seu agente:

### Teste 1: Consulta de gastos
- **Pergunta:** "Quanto gastei com alimentação?"
- **Resposta esperada:** Valor baseado no `transacoes.csv`
- **Resultado:** [X] Correto  [ ] Incorreto

### Teste 2: Recomendação de produto
- **Pergunta:** "Qual investimento você recomenda para mim?"
- **Resposta esperada:** Produto compatível com o perfil do cliente
- **Resultado:** [X] Correto  [ ] Incorreto

### Teste 3: Pergunta fora do escopo
- **Pergunta:** "Qual a previsão do tempo?"
- **Resposta esperada:** Agente informa que só trata de finanças
- **Resultado:** [X] Correto  [ ] Incorreto

### Teste 4: Informação inexistente
- **Pergunta:** "Quanto rende o produto XYZ?"
- **Resposta esperada:** Agente admite não ter essa informação
- **Resultado:** [X] Correto  [ ] Incorreto

---

## Resultados

Após os testes, registre suas conclusões:

**O que funcionou bem:**
- o agente (eco) não teve oscilações, assumiu quando não sabia de algo e se manteve no foco de ser um educador financeiro, se mantendo no roteiro de, após a sua permissão, apenas sugerir e explicar a melhor opção financeira para o cliente baseando no seu histórico financeiro

**O que pode melhorar:**
- mais opções de como o cliente pode dividir a sua renda líquida de forma customizável, no momento o eco apenas apresenta e explica o método 50/30/20, mas quando informado que no próximo mês o cliente terá dividas á mais que o mês passado ele continua indicando referente ao que já está registrado na `data/transacoes.csv`

---
