# 01 — Iteração de prompts para documentação técnica

[Voltar aos estudos](./README.md)

## Objetivo do exercício

Produzir uma introdução didática sobre armazenamento de senhas para desenvolvedores iniciantes e comparar duas formas de especificar a resposta.

## Primeira versão — transcrição do trabalho

```text
Atue como um Engenheiro de Segurança da Informação Sênior. Sua
tarefa é escrever um parágrafo introdutório para a nova documentação
interna do nosso sistema de autenticação. Tarefa: Escreva um
parágrafo justificando a migração do uso de hashes simples (como
MD5) para algoritmos mais seguros que utilizam "Salt" e "Key
Stretching" (como o bcrypt). Requisitos: Público-alvo: Desenvolvedores
júnior da equipe. Tom: Técnico, formal e didático. Conteúdo: Explique
brevemente o risco do MD5 (ex: força bruta e rainbow tables) e por que
o bcrypt com Salt resolve esse problema. Extensão: Entre 5 e 8 linhas.
Evite: Explicações excessivamente matemáticas; foque na aplicação
prática do dia a dia. Formato de saída: Apenas o parágrafo gerado, sem
saudações ou comentários adicionais.
```

## Refinamento — transcrição do trabalho

```text
Contexto: Você está elaborando a documentação técnica interna para a
nossa equipe de desenvolvedores juniores. O objetivo é justificar
tecnicamente a migração do uso de hashes obsoletos (como MD5) para o
padrão seguro utilizando bcrypt. Tarefa: Escreva um parágrafo introdutório
para essa documentação seguindo RIGOROSAMENTE as regras abaixo: 1.
Formato e Estrutura (Exatamente 4 frases): Frase 1: Defina a vulnerabilidade
de hashes rápidos (ex: suscetibilidade a força bruta e rainbow tables). Frase
2: Explique o conceito de "Salt" incluindo obrigatoriamente uma
microdefinição embutida (ex: Salt (dado aleatório único anexado à senha)).
Frase 3: Explique o "Key Stretching" focando na lentidão intencional para
encarecer o ataque computacional. Frase 4: Conclua com uma diretriz
normativa e imperativa de segurança para a equipe seguir. 2. Tom de voz e
Restrições: Tom: Técnico, formal, imperativo e didático. Restrição Negativa:
NÃO afirme que o sistema será "100% seguro" ou "in-hackeável". Qualifique o
nível de proteção usando termos realistas como "mitiga significativamente"
ou "eleva o custo computacional". 3. Etapa de Auto-validação (Silenciosa):
Antes de gerar a saída, faça um checklist internamente (não imprima): O texto
possui exatamente 4 frases? Contém a microdefinição de Salt? Evitou
promessas de segurança absoluta? Formato de saída final: Se todas as
respostas forem "sim", imprima APENAS o parágrafo gerado, sem saudações
ou comentários adicionais.
```

## O que mudou

| Escolha | Primeira versão | Versão refinada |
| --- | --- | --- |
| Extensão | Entre cinco e oito linhas | Exatamente quatro frases |
| Organização | Conteúdos solicitados em conjunto | Uma função definida para cada frase |
| Linguagem | Técnica e didática | Microdefinições e conclusão imperativa |
| Limites | Evitar excesso de matemática | Evitar promessas de segurança absoluta |

O PDF contém capturas das duas interações e uma análise comparativa. A análise relata maior separação dos conceitos e menor fluidez na estrutura rígida. Isso é uma avaliação qualitativa do exercício, sem experimento controlado ou amostra de múltiplas respostas.

## Revisão para o portfólio

A hipótese de que a estrutura rígida aumentaria o controle é válida como objeto de teste. A afirmação original de que isso anularia alucinações não foi comprovada. Pedir autoverificação ao modelo também não equivale a uma validação externa ou a um registro de auditoria.

O conteúdo técnico dos prompts foi preservado como material histórico. Para orientar uma implementação atual, consultar as recomendações de armazenamento de senhas, em vez de tratar a escolha do exercício como regra universal. [Referência: OWASP Password Storage](https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html).

## Próximo experimento proposto

Executar as duas versões sob condições registradas, repetir as gerações e avaliar cobertura dos requisitos, clareza e erros factuais com uma rubrica. Comparar também uma terceira versão com requisitos de conteúdo, sem contagem rígida de frases.

**Fonte:** Bruno Delmondes - Engenharia de prompt - atv1 (2).pdf, páginas 4–8. A organização não reexecutou os prompts nem inventou novas respostas.
