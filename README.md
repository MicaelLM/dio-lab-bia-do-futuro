# 🎓 Eco — Educador Financeiro Inteligente

> Agente de IA Generativa que ensina conceitos de finanças pessoais de forma simples e personalizada, usando os dados do cliente como exemplos práticos.

## 💡 Sobre

O Eco **explica**, não recomenda. Ele traduz conceitos como reserva de emergência, tipos de investimento e análise de gastos em linguagem simples, sempre com exemplos baseados no perfil do usuário.

| Faz ✅ | Não faz ❌ |
|---|---|
| Explica conceitos financeiros | Recomendar investimentos específicos |
| Usa dados do cliente como exemplo | Acessar dados bancários sensíveis |
| Responde dúvidas sobre produtos | Substituir um profissional certificado |
| Analisa padrões de gastos | — |

## 🏗️ Arquitetura

```
Usuário → Streamlit → Ollama (LLM local) ⇄ Base de Conhecimento → Resposta Educativa
```

**Stack:** Streamlit (interface) · Ollama com `gpt-oss` (LLM local) · JSON/CSV (dados mockados)

## 📁 Estrutura

```
├── data/    # Perfil, transações, histórico e produtos financeiros (mock)
├── docs/    # Documentação do agente, prompts, métricas e pitch
├── src/
│   └── app.py   # Aplicação Streamlit
```

## 🚀 Como executar

```bash
# 1. Instalar e subir o Ollama (ollama.com)
ollama pull gpt-oss
ollama serve

# 2. Instalar dependências
pip install streamlit pandas requests

# 3. Rodar o Eco
streamlit run src/app.py
```

## 🎯 Exemplo

**Pergunta:** "Onde estou gastando mais?"
**Eco:** "Olhando suas transações de outubro, sua maior despesa é moradia (R$ 1.380), seguida de alimentação (R$ 570) — juntas, quase 80% dos seus gastos. Quer que eu explique algumas estratégias de organização?"

## 📊 Avaliação

| Métrica | Objetivo |
|---|---|
| Assertividade | Responde ao que foi perguntado? |
| Segurança | Evita alucinação/invenção de dados? |
| Coerência | Resposta adequada ao perfil do cliente? |

## 🎬 Diferenciais

- **Personalizado:** usa os dados do próprio cliente nos exemplos
- **100% local:** roda via Ollama, sem enviar dados a APIs externas
- **Educativo:** foco em ensinar, não em vender
- **Seguro:** estratégias anti-alucinação documentadas

## 📝 Documentação

Documentação técnica completa, estratégias de prompt e casos de teste em [`docs/`](docs).

---
Desafio de projeto — Digital Innovation One (DIO)
