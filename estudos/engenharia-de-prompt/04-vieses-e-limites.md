# 04 — Vieses e limites de uso da IA

[Voltar aos estudos](./README.md)

## Cenário acadêmico

O exercício analisa uma proposta de triagem de currículos e discute como padrões históricos, origem institucional e vocabulário podem influenciar recomendações.

O objetivo desta apresentação é registrar a análise crítica. Não há agente de recrutamento implementado, classificação de pessoas reais ou validação de imparcialidade nesta pasta.

## Riscos e medidas discutidas

| Risco identificado no trabalho | Medida proposta | O que ainda precisa ser demonstrado |
| --- | --- | --- |
| Reprodução de padrões históricos | Redução de dados identificadores e revisão dos dados utilizados | Avaliar se o resultado continua associado a características ou indicadores indiretos. |
| Preferência por instituições conhecidas | Rever critérios e ampliar a diversidade dos exemplos | Medir o comportamento em casos comparáveis e documentar o método. |
| Dependência de palavras-chave | Avaliar sinônimos e exigir justificativas apoiadas no conteúdo | Testar descrições equivalentes e verificar a consistência das respostas. |
| Instruções adversariais nos documentos | Separar o conteúdo recebido das regras do sistema | Executar testes e aplicar controles além de instruções no prompt. |

## Revisão das conclusões originais

Remover nomes, solicitar justificativas ou escrever regras éticas não comprova que os vieses foram eliminados. O material não apresenta conjunto de avaliação, resultados de testes ou auditoria independente. A justificativa de conformidade com a LGPD no PDF é uma argumentação acadêmica, não uma análise jurídica validada.

O exemplo original pede uma classificação de compatibilidade e um campo de confiança. Esses campos não são apresentados aqui como instrumentos validados para decisões de contratação. Uma evolução do estudo deve delimitar o apoio à revisão humana, os critérios relevantes e a possibilidade de contestar resultados.

## Como avançar no estudo

1. Usar exemplos inteiramente fictícios, com critérios explícitos para comparação.
2. Separar evidências encontradas, informações ausentes e interpretações do modelo.
3. Definir avaliação e supervisão antes de qualquer uso real.
4. Registrar falhas e revisar as medidas propostas sem declarar garantias absolutas.

Sobre instruções adversariais, a [OWASP](https://genai.owasp.org/llmrisk/llm01-prompt-injection/) descreve controles complementares e testes. Isso sustenta tratar o prompt como parte da proposta, sem presumir proteção completa.

**Fonte:** Engenharia de prompt - Atividade 04 - Aula 04 - Bruno.pdf, páginas 4–6. O prompt de triagem original não foi executado e não foi publicado como serviço operacional.
