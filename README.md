# Prompt Engineering Lab

Coleção de prompts bem estruturados que testei em modelos de linguagem (Claude, ChatGPT, Gemini), com a técnica usada em cada um e o que observei nos testes.

## Estrutura de um bom prompt

1. **Papel:** quem o modelo deve ser.
2. **Contexto:** o que ele precisa saber.
3. **Tarefa:** o que fazer, de forma específica.
4. **Formato de saída:** como responder (lista, tabela, JSON).
5. **Restrições:** o que evitar ou limites de tamanho.

---

## 1. Resumo de texto com formato fixo
**Técnica:** formato de saída definido.

```
Você é um assistente de estudos. Resuma o texto abaixo em exatamente 3 tópicos curtos e depois escreva 1 pergunta de revisão sobre ele.

Texto: [COLE O TEXTO AQUI]
```
**Meu resultado:** _(preencher depois de testar)_

## 2. Explicar um conceito para iniciantes
**Técnica:** papel + público-alvo + analogia.

```
Você é um professor paciente. Explique [CONCEITO] para um estudante de 1º semestre, usando uma analogia do dia a dia e no máximo 120 palavras. Termine com um exemplo prático.
```
**Meu resultado:** _(preencher depois de testar)_

## 3. Classificar mensagens de clientes
**Técnica:** few-shot (exemplos dentro do prompt).

```
Classifique a mensagem do cliente como: ELOGIO, RECLAMACAO ou DUVIDA. Responda só com a categoria.

Mensagem: "Meu pedido chegou frio" -> RECLAMACAO
Mensagem: "Vocês entregam no domingo?" -> DUVIDA
Mensagem: "Entrega rápida, amei!" -> ELOGIO

Mensagem: "[NOVA MENSAGEM]" ->
```
**Meu resultado:** _(preencher depois de testar)_

## 4. Resolver problemas passo a passo
**Técnica:** raciocínio em etapas.

```
Resolva o problema abaixo pensando passo a passo. Mostre cada etapa e, no final, dê a resposta em uma linha começando com "RESPOSTA:".

Problema: [PROBLEMA]
```
**Meu resultado:** _(preencher depois de testar)_

## 5. Extrair dados em JSON
**Técnica:** saída estruturada.

```
Extraia do texto abaixo o nome, o valor e a data. Responda apenas com um JSON válido no formato {"nome": "", "valor": 0, "data": ""}. Se faltar algum dado, use null.

Texto: [TEXTO]
```
**Meu resultado:** _(preencher depois de testar)_

## 6. Revisão do próprio resultado
**Técnica:** auto-crítica.

```
Escreva um e-mail pedindo [ASSUNTO]. Depois, revise o e-mail apontando 2 pontos que podem melhorar e reescreva a versão final.
```
**Meu resultado:** _(preencher depois de testar)_

---

## Aprendizados

- Prompts específicos geram respostas mais úteis do que pedidos vagos.
- Mostrar exemplos (few-shot) melhora muito a consistência.
- Definir o formato de saída facilita usar a resposta em código.

## Autor

**[kariny rose vaz]**, estudante de Sistemas de Informação.
