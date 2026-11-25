# Checklist

## Objetivo

Este documento define a lista de verificação que deverá ser utilizada antes de considerar qualquer etapa, funcionalidade ou módulo do projeto como concluído.

Seu objetivo é garantir qualidade, organização, consistência e conformidade com a Constituição de Desenvolvimento e com os demais documentos do projeto.

---

## Planejamento

Antes de iniciar o desenvolvimento, verificar:

* o problema está claramente definido;

* o objetivo da etapa ou funcionalidade está documentado;

* o escopo da versão atual está definido;

* as funcionalidades futuras estão separadas das funcionalidades da versão atual;

* a etapa está de acordo com a Arquitetura e a Arquitetura de Dados;

* as regras e decisões importantes estão documentadas antes da implementação.

---

## Arquitetura

Verificar se:

* a estrutura do projeto está organizada;

* cada arquivo possui uma responsabilidade principal;

* cada módulo possui uma responsabilidade clara;

* os componentes de coleta, processamento, análise, filtros e apresentação estão corretamente separados;

* os arquivos compartilhados estão corretamente separados;

* os ambientes de desenvolvimento e operação estão respeitados;

* nenhuma alteração criou dependência desnecessária entre módulos.

---

## Dados

Verificar se:

* os dados possuem estrutura definida;

* o Item continua sendo a unidade fundamental de análise;

* oportunidades, lotes, grupos e itens estão corretamente relacionados;

* os dados originais foram preservados quando necessário;

* os dados processados estão separados dos dados originais;

* categorias, subcategorias, filtros e configurações não foram desnecessariamente fixados no código;

* não existem dados inventados ou preenchidos sem fonte definida;

* duplicidades relevantes foram tratadas;

* as informações importantes possuem origem identificável;

* alterações na estrutura de dados foram devidamente documentadas.

---

## Desenvolvimento

Verificar se:

* cada funcionalidade foi implementada individualmente;

* nenhuma etapa foi pulada;

* nenhuma funcionalidade ficou parcialmente implementada;

* não existem trechos de código temporários esquecidos;

* as funcionalidades seguem o fluxo de desenvolvimento definido;

* a implementação respeita as decisões arquiteturais já estabelecidas;

* o sistema continua preparado para evolução futura.

---

## Código

Verificar se:

* o código está organizado;

* os nomes são claros;

* não existe duplicação desnecessária;

* as funções possuem responsabilidades bem definidas;

* os módulos possuem responsabilidades claras;

* a leitura do código está simples;

* o código segue os padrões definidos no documento de Padrões de Código;

* não foram adicionadas bibliotecas, serviços ou estruturas desnecessárias;

* informações sensíveis, credenciais e chaves de acesso não estão expostas no código.

---

## Coleta de Dados

Verificar se:

* as fontes de dados estão corretamente configuradas;

* a coleta respeita as fontes e os critérios definidos;

* os dados coletados possuem origem identificável;

* oportunidades duplicadas não estão sendo criadas desnecessariamente;

* falhas de coleta são identificadas e registradas;

* a coleta não altera indevidamente os dados originais;

* o sistema consegue continuar sua operação após falhas recuperáveis;

* a coleta está de acordo com as regras definidas para o projeto.

---

## Análise e Inteligência

Verificar se:

* os itens foram corretamente identificados;

* a classificação dos itens está coerente;

* os critérios de compatibilidade estão sendo aplicados corretamente;

* o percentual de compatibilidade possui justificativa;

* os filtros selecionados estão sendo respeitados;

* a capacidade de fornecimento está sendo considerada quando aplicável;

* localização, entrega, prazo e demais critérios relevantes estão sendo considerados;

* a análise não apresenta como certeza aquilo que é apenas estimativa;

* o sistema não inventa informações ausentes nos dados de origem.

---

## Inteligência de Preços

Verificar se:

* os preços históricos utilizados possuem origem identificável;

* os dados históricos utilizados são comparáveis ao item analisado;

* unidades, quantidades e especificações foram consideradas na comparação;

* diferenças relevantes entre os itens foram consideradas;

* os preços foram tratados e normalizados quando necessário;

* a sugestão de preço possui justificativa baseada nos dados disponíveis;

* a qualidade das evidências utilizadas está identificada;

* o sistema não inventa preços quando não existem dados suficientes;

* os custos reais cadastrados pelo usuário estão sendo considerados quando aplicável;

* as simulações de proposta estão separadas da decisão final do usuário.

---

## Análise Financeira

Verificar se:

* o custo de aquisição foi considerado quando disponível;

* frete foi considerado quando aplicável;

* impostos foram considerados quando aplicável;

* outros custos relevantes foram considerados;

* a margem estimada foi calculada corretamente;

* o resultado financeiro estimado está coerente com os dados utilizados;

* nenhuma margem ou custo foi inventado sem informação ou regra definida;

* os valores apresentados deixam claro quando são estimativas.

---

## Inteligência Artificial

Verificar se:

* todas as alterações seguiram as Regras para IA;

* todas as alterações foram validadas antes da próxima etapa;

* nenhuma modificação desnecessária foi realizada;

* nenhuma decisão arquitetural importante foi tomada sem análise prévia;

* toda alteração ficou claramente documentada;

* a IA respeitou os documentos oficiais do projeto;

* a IA não substituiu regras do sistema por interpretações próprias sem autorização.

---

## Testes

Verificar se:

* todas as funcionalidades foram testadas;

* os fluxos principais funcionam corretamente;

* os erros conhecidos foram corrigidos;

* não existem erros não tratados;

* não existem mensagens de erro inesperadas nos logs;

* a coleta foi testada;

* o processamento dos dados foi testado;

* os filtros foram testados;

* a análise de compatibilidade foi testada;

* os cálculos financeiros foram testados;

* a inteligência de preços foi testada;

* os resultados apresentados correspondem aos dados processados.

---

## Operação

Antes de considerar o sistema pronto para operação contínua, verificar se:

* o ambiente de operação está corretamente configurado;

* o robô consegue executar suas tarefas de forma contínua;

* as falhas são identificadas e registradas;

* os processos podem ser reiniciados quando necessário;

* os dados coletados continuam sendo armazenados corretamente;

* o sistema não depende do computador de desenvolvimento para executar sua rotina normal;

* as atualizações realizadas no ambiente de desenvolvimento foram validadas antes de serem disponibilizadas no ambiente de operação.

---

## Documentação

Verificar se:

* a documentação do projeto está atualizada;

* as decisões importantes foram registradas;

* os arquivos Markdown refletem a situação atual do projeto;

* alterações importantes na arquitetura foram documentadas;

* alterações importantes na estrutura de dados foram documentadas;

* novas funcionalidades foram refletidas na documentação correspondente;

* não existem documentos contraditórios ou desatualizados sobre uma mesma regra.

---

## Segurança

Verificar se:

* chaves de API e credenciais não estão expostas;

* informações sensíveis não estão armazenadas diretamente no código;

* acessos externos estão protegidos;

* arquivos de configuração sensíveis estão corretamente tratados;

* logs não expõem informações sensíveis desnecessariamente;

* as alterações não criaram vulnerabilidades conhecidas;

* os dados importantes possuem proteção adequada ao contexto do projeto.

---

## Publicação e Operação

Antes de disponibilizar uma nova versão para operação, verificar se:

* o projeto está estável;

* os testes foram concluídos;

* a documentação está atualizada;

* a versão foi validada no ambiente de desenvolvimento;

* a implantação no ambiente de operação foi realizada corretamente;

* as funcionalidades existentes continuam funcionando;

* o projeto segue integralmente a Constituição de Desenvolvimento e os documentos oficiais.

---

## Aprovação Final

Uma etapa, funcionalidade, módulo ou versão somente poderá ser considerada concluída quando os itens aplicáveis deste checklist forem atendidos.

Nenhuma funcionalidade deverá ser considerada concluída apenas porque o código está funcionando.

A conclusão deverá considerar também arquitetura, dados, segurança, testes, documentação e conformidade com as regras do projeto.
