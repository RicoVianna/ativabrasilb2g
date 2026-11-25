# Arquitetura

## Objetivo

Este documento define a arquitetura padrão utilizada em todos os projetos.

Seu objetivo é criar uma estrutura previsível, organizada, simples de manter e fácil de compreender por pessoas e Inteligências Artificiais.

Toda nova aplicação deverá seguir esta arquitetura, salvo quando existir uma justificativa técnica para utilizar uma estrutura diferente.

---

## Princípios Arquiteturais

### 1. Organização antes da implementação

A estrutura do projeto deverá ser definida antes da criação das funcionalidades.

Nunca iniciar um projeto escrevendo código sem possuir uma organização mínima.

---

### 2. Uma responsabilidade para cada arquivo

Cada arquivo deverá possuir uma responsabilidade principal.

Um arquivo não deverá concentrar diversas funcionalidades diferentes.

---

### 3. Uma responsabilidade para cada página

Cada página deverá possuir sua própria lógica principal.

Sempre que possível, cada página deverá possuir:

- um arquivo HTML;
- um arquivo JavaScript principal;
- um arquivo CSS próprio.

---

### 4. Arquivos globais

Arquivos que pertencem ao projeto inteiro poderão existir separadamente.

Exemplos:

- configuração;
- autenticação;
- utilitários;
- serviços compartilhados.

Esses arquivos não pertencem a uma página específica.

---

### 5. Modularização

Quando uma funcionalidade crescer além do razoável, ela deverá ser dividida em módulos menores.

A modularização deverá reduzir a complexidade, nunca aumentá-la.

---

### 6. Baixo acoplamento

Sempre que possível, uma página deverá depender o mínimo possível de outras páginas.

Cada parte do sistema deverá funcionar de forma independente.

---

### 7. Facilidade para manutenção

A arquitetura deverá permitir localizar rapidamente:

- onde uma funcionalidade está;
- onde um problema ocorreu;
- onde uma melhoria deverá ser implementada.

---

### 8. Arquitetura amigável para Inteligências Artificiais

A organização do projeto deverá facilitar o entendimento pelas IAs.

Arquivos excessivamente grandes, responsabilidades misturadas e estruturas confusas deverão ser evitados.

---

### 9. Evolução controlada

A arquitetura poderá evoluir ao longo do tempo.

Entretanto, qualquer mudança deverá tornar o projeto mais simples, mais organizado e mais fácil de manter.