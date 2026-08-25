# Base de Conhecimento

## Dados Utilizados

| Arquivo | Formato | Função do eco |
|---------|---------|---------------------|
| `historico_atendimento.csv` | CSV | Contextualizar interações anteriores dando continuidade ao atendimento com eficiência |
| `perfil_investidor.json` | JSON | recomendações de serviços personalizadas referente a situação de cada cliente visando economia |
| `produtos_financeiros.json` | JSON | apresentar os serviços disponíveis de economia forma educacional ao cliente |
| `transacoes.csv` | CSV | Analisar padrão de gastos do cliente e mostrar uma alternativa econômica de renda |


---

## Estratégia de Integração

### Como os dados são carregados?
> Descreva como seu agente acessa a base de conhecimento.

[ex: Os JSON/CSV são carregados no início da sessão e incluídos no contexto do prompt]

### Como os dados são usados no prompt?
> Os dados vão no system prompt? São consultados dinamicamente?

[Sua descrição aqui]

---

## Exemplo de Contexto Montado

> Mostre um exemplo de como os dados são formatados para o agente.

```
Dados do Cliente:
- Nome: João Silva
- Perfil: Moderado
- Saldo disponível: R$ 5.000

Últimas transações:
- 01/11: Supermercado - R$ 450
- 03/11: Streaming - R$ 55
...
```
