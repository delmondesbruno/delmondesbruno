# 02 — Revisão crítica de código sugerido por IA

[Voltar aos estudos](./README.md)

## Problema estudado

O cenário acadêmico descreve uma sugestão de uso de MD5 para armazenar senhas. O trabalho discute o risco de aceitar uma resposta de IA sem verificar sua adequação e propõe requisitos mais explícitos.

## Prompt proposto no exercício

```text
Atue como um engenheiro de software especializado em segurança da
informação. Preciso de uma função em Python para fazer hash de senhas de
usuários em um sistema de autenticação. Requisitos obrigatórios: - Utilize o
algoritmo bcrypt (ou Argon2, se preferir, mas justifique a escolha). - Inclua a
geração de um "salt" aleatório e único para cada senha. - A função deve
receber a senha em texto puro e retornar o hash gerado (já com o salt
incorporado, como o bcrypt faz por padrão). - Crie também uma função
separada para verificar se uma senha fornecida corresponde ao hash
armazenado. - Adicione comentários explicando cada parte do código,
especialmente os conceitos de segurança envolvidos. - O código deve seguir
as boas práticas da linguagem Python (PEP 8). - Inclua um exemplo de uso
básico no final. Contexto: O sistema será usado em produção, então a
segurança é prioridade. Evite algoritmos antigos ou inseguros como MD5 ou
SHA1. Explique rapidamente por que bcrypt (ou Argon2) é a escolha correta
hoje.
```

## O que o material demonstra

- Definição de objetivo, contexto e requisitos para a resposta.
- Separação entre gerar um hash e verificar uma senha.
- Preocupação com revisão humana, comentários e exemplos.

O PDF não contém uma implementação Python completa nem resultados de testes de autenticação. Portanto, esta atividade é apresentada como especificação e análise, sem atribuir ao autor uma implementação que não está anexada.

## Pontos a revisar

- Um pedido bem especificado reduz ambiguidades, mas não comprova a segurança do código que será gerado.
- A adequação do algoritmo, seus parâmetros, a biblioteca e o comportamento precisam ser revisados e testados na implementação.
- As citações acadêmicas a Barcaui e Carraro no texto original precisam de referência bibliográfica completa antes de serem reutilizadas como citações verificadas.

Para aprofundamento técnico, usar a [OWASP Password Storage Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html). A escolha de bcrypt no exercício é mantida como contexto histórico; a referência atual orienta a seleção entre algoritmos e seus parâmetros.

**Fonte:** Aula02 - Engenharia de Prompt - atv2  (2).pdf, páginas 4–5. Nenhum código foi gerado ou executado nesta organização do portfólio.
