# Fluxo de Desenvolvimento

## Objetivo

Este documento define a sequência padrão utilizada para desenvolver todos os projetos.

O objetivo é reduzir erros, manter a organização e facilitar o trabalho conjunto entre o desenvolvedor e as Inteligências Artificiais.

Todas as etapas deverão ser executadas na ordem definida neste documento, salvo quando existir justificativa técnica para seguir outro fluxo.

---

## Etapa 1 - Planejamento

Antes de qualquer linha de código, definir claramente:

- o problema que será resolvido;
- o objetivo do projeto;
- o público-alvo;
- as funcionalidades da primeira versão (MVP);
- o que ficará para versões futuras.

Nenhum projeto deverá começar diretamente pela programação.

---

## Etapa 2 - Estrutura do Projeto

Criar a estrutura inicial do projeto.

Definir:

- páginas;
- arquivos;
- organização das pastas;
- documentação inicial.

Toda a estrutura deverá ser organizada antes da implementação.

---

## Etapa 3 - Interface

Construir inicialmente a interface.

Priorizar:

- HTML;
- estrutura das páginas;
- navegação;
- organização visual.

Nesta etapa, não implementar regras de negócio complexas.

---

## Etapa 4 - Estilização

Aplicar o CSS.

Priorizar:

- organização visual;
- responsividade;
- consistência entre as páginas.

Evitar ajustes prematuros de detalhes estéticos.

---

## Etapa 5 - Funcionalidades

Implementar a lógica da aplicação.

Adicionar uma funcionalidade por vez.

Cada funcionalidade deverá ser concluída antes do início da próxima.

---

## Etapa 6 - Integrações

Somente após o funcionamento correto da interface e da lógica principal deverão ser realizadas integrações externas.

Exemplos:

- autenticação;
- banco de dados;
- pagamentos (nesse projeto não haverá pagamentos);
- serviços externos;
- APIs.

---

## Etapa 7 - Testes

Testar todas as funcionalidades implementadas.

Corrigir problemas antes da criação de novas funcionalidades.

Nunca acumular erros para corrigir posteriormente.

---

## Etapa 8 - Refatoração

Após o funcionamento correto da aplicação, revisar:

- organização;
- nomes;
- duplicação de código;
- modularização;
- clareza.

Refatorar apenas quando isso realmente melhorar o projeto.

---

## Etapa 9 - Publicação

Somente publicar quando:

- todas as funcionalidades previstas estiverem concluídas;
- os testes forem satisfatórios;
- a documentação estiver atualizada.

---

## Regra Geral

Sempre concluir uma etapa antes de iniciar a próxima.

Evitar trabalhar simultaneamente em diversas funcionalidades ou diversas partes do sistema.

A simplicidade e a organização deverão prevalecer durante todo o desenvolvimento.