# Regras para IA

## Objetivo

Este documento define as regras que deverão ser seguidas por qualquer Inteligência Artificial durante o desenvolvimento dos projetos.

O objetivo é garantir respostas organizadas, previsíveis, detalhadas e compatíveis com a forma de trabalho do desenvolvedor.

Todas as IAs deverão seguir estas regras durante todo o desenvolvimento do projeto.

---

## Regra 1 - Um passo por mensagem

Cada resposta deverá conter apenas um passo operacional.

O próximo passo somente poderá ser apresentado após a confirmação de que o passo anterior foi executado e validado.

Nunca apresentar múltiplos passos sequenciais na mesma resposta.

---

## Regra 2 - Alterações extremamente específicas

Sempre que houver necessidade de alterar um arquivo, informar claramente:

- qual arquivo será alterado;
- se o código será criado, substituído ou removido;
- o local exato da alteração;
- abaixo de qual função;
- acima de qual função;
- dentro de qual bloco;
- ou entre quais linhas, quando possível.

Nunca utilizar instruções genéricas como:

- "adicione este código";
- "cole em qualquer lugar";
- "insira próximo ao final".

Toda alteração deverá possuir uma localização precisa.

---

## Regra 3 - Preservação da arquitetura

Antes de sugerir qualquer alteração, verificar se ela respeita:

- a Filosofia;
- a Arquitetura;
- o Fluxo de Desenvolvimento;
- os Padrões de Código.

Nenhuma sugestão deverá quebrar os padrões definidos pela Constituição.

---

## Regra 4 - Explicações objetivas

As explicações deverão ser claras, objetivas e suficientes para que o desenvolvedor compreenda o motivo da alteração.

Evitar textos excessivamente longos quando uma explicação simples for suficiente.

---

## Regra 5 - Priorizar simplicidade

Sempre sugerir inicialmente a solução mais simples.

Somente utilizar soluções mais complexas quando forem realmente necessárias.

---

## Regra 6 - Respeitar o nível de conhecimento do desenvolvedor

Considerar que o desenvolvedor está em processo de aprendizagem.

Evitar assumir conhecimentos avançados sem explicação.

Sempre que necessário, explicar conceitos importantes de forma simples.

---

## Regra 7 - Manter consistência

Sempre utilizar os mesmos padrões adotados no restante do projeto.

Evitar criar novas convenções sem necessidade.

---

## Regra 8 - Indentação

Todos os exemplos de código deverão utilizar indentação de 4 espaços.

A organização visual deverá facilitar a leitura e a manutenção.

---

## Regra 9 - Não realizar alterações desnecessárias

Modificar apenas o que for solicitado ou o que for indispensável para o correto funcionamento da solução.

Evitar alterar partes do projeto que não estejam relacionadas ao problema em questão.

---

## Regra 10 - Validar antes de continuar

Após cada alteração importante, aguardar a confirmação do desenvolvedor antes de prosseguir para a próxima etapa.

Nenhuma nova implementação deverá ser iniciada sem a validação da etapa anterior.

---

## Regra Geral

Sempre priorizar:

- organização;
- clareza;
- previsibilidade;
- simplicidade;
- facilidade de manutenção;
- compatibilidade com Inteligências Artificiais.

Todas as respostas deverão respeitar integralmente esta Constituição de Desenvolvimento.