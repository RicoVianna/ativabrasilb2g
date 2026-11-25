# Padroes de Codigo

## Objetivo

Este documento define os padrões utilizados durante o desenvolvimento do código.

Seu objetivo é manter todos os projetos consistentes, organizados, fáceis de compreender e simples de manter.

Todos os projetos deverão seguir estes padrões.

---

## Padrão 1 - Clareza acima de tudo

Todo código deverá ser escrito para ser facilmente compreendido.

Um código simples e legível possui prioridade sobre um código excessivamente sofisticado.

---

## Padrão 2 - Nomes descritivos

Variáveis, funções, arquivos e demais elementos deverão possuir nomes que descrevam claramente sua finalidade.

Evitar nomes genéricos ou abreviações desnecessárias.

---

## Padrão 3 - Uma responsabilidade por função

Cada função deverá executar apenas uma responsabilidade principal.

Funções excessivamente grandes deverão ser divididas em funções menores.

---

## Padrão 4 - Uma responsabilidade por arquivo

Cada arquivo deverá possuir um objetivo claramente definido.

Sempre que possível, evitar misturar responsabilidades diferentes dentro do mesmo arquivo.

---

## Padrão 5 - Organização do código

O código deverá seguir uma ordem lógica.

Sempre que possível, organizar os arquivos nesta sequência:

- constantes;
- configurações;
- variáveis globais;
- inicialização;
- funções auxiliares;
- funções principais;
- eventos;
- execução inicial.

---

## Padrão 6 - Evitar duplicação

Sempre que uma lógica for reutilizada em diferentes locais, avaliar a criação de uma função reutilizável.

Evitar duplicação desnecessária de código.

---

## Padrão 7 - Comentários

Comentários deverão explicar o motivo de uma implementação.

Evitar comentários que apenas repitam exatamente o que o código já demonstra.

---

## Padrão 8 - Modularização

Quando um arquivo começar a crescer excessivamente, avaliar sua divisão em módulos menores.

A modularização deverá facilitar a manutenção.

Nunca deverá aumentar a complexidade.

---

## Padrão 9 - Consistência

Todos os arquivos deverão seguir o mesmo padrão de organização.

A consistência possui prioridade sobre preferências individuais.

---

## Padrão 10 - Preparação para manutenção

Todo código deverá ser escrito considerando futuras alterações.

Sempre pensar que outro desenvolvedor — ou uma Inteligência Artificial — precisará compreender rapidamente aquele arquivo.

---

## Regra Geral

Antes de considerar uma funcionalidade concluída, verificar se o código permanece:

- organizado;
- simples;
- consistente;
- legível;
- modular;
- fácil de manter.