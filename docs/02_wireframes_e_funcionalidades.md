# DOCUMENTO DE WIREFRAMES, COMPONENTES E FUNCIONALIDADES (ETAPA 2)
**Projeto:** Ativa Brasil Soluções B2G (`ativabrasilb2g.com.br`)  
**Abordagem de Construção:** Vibe Coding / Arquitetura Estática de Alta Performance (Sem Backend/Banco de Dados próprio)  
**Integração:** Seguir rigorosamente as regras técnicas definidas em `00_constituicao_desenvolvimento.md` e a identidade visual de `01_diretrizes_identidade_e_sitemap.md`.

---

## 1. REGRAS DE ARQUITETURA E VIBE CODING (PARA A IA GERADORA DE CÓDIGO)

1. **Zero Dependência de Servidor/Banco de Dados:** Todo o site deve funcionar de forma autônoma no front-end (HTML5, CSS3/Tailwind e JavaScript limpo), garantindo carregamento instantâneo e hospedagem simples.
2. **Design Modular e Manutenível:** Código organizado, comentado e fácil de editar futuramente (ex: fácil troca de links de checkout da Hotmart, adição de novos cursos ou novas categorias de produtos B2G sem quebrar o layout).
3. **Responsividade Absoluta (Mobile-First & Desktop Executivo):** O layout deve ser impecável tanto na tela widescreen de um pregoeiro no computador do órgão público quanto no smartphone de um aluno acessando via Instagram/WhatsApp.
4. **Estética Editorial sem Catálogo:** O site é institucional e de curadoria executiva, não um e-commerce ou catálogo de produtos. Não criar páginas/componentes de catálogo de mercadorias, fichas técnicas de produtos, carrinho de compras ou fotos de itens avulsos; priorizar tipografia limpa, fotografia corporativa/arquitetônica sóbria, ícones minimalistas e micro-interações sutis.

---

## 2. COMPONENTES GLOBAIS (PRESENTES EM TODO O SITE)

### 2.1. Splash Screen Minimalista (Abertura)
* **Comportamento:** Exibida apenas na primeira entrada da sessão (`sessionStorage` para não irritar o usuário se ele navegar entre páginas internas). Duração total: `1.5 segundos`.
* **Visual:**
  * Fundo: Azul Marinho Profundo (`#0A192F`).
  * Centro: Logotipo tipográfico **Ativa Brasil** em branco (`#F8FAFC`) + subtítulo discreto *"Soluções B2G & Capacitação Estratégica"*.
  * Barra de Progresso: Linha horizontal ultrafina (`2px` de altura, largura máxima `220px`) logo abaixo do subtítulo, preenchendo suavemente de `0%` a `100%` em Verde Institucional (`#047857`).
  * Saída: *Fade-out* suave revelando a página principal.

### 2.2. Cabeçalho (Navbar Fixa / Sticky)
* **Layout:** Fundo Branco Gelo (`#F8FAFC`) com borda inferior sutil (`1px solid #E2E8F0`), altura limpa (`80px`).
* **Esquerda:** Logotipo **Ativa Brasil** (com subtítulo discreto *"Soluções B2G & Capacitação Estratégica"*).
* **Centro (Links de Navegação):** `Início` | `Fornecimento B2G` | `Capacitação` | `Sobre Nós` | `Contato`.
* **Direita (Botões de Ação Dual):**
  * **Botão Secundário (Outline):** `Portal do Aluno` *(link externo direto para a área de membros da Hotmart)*.
  * **Botão Primário (Sólido `#047857`):** `Solicitar Cotação B2G` *(rola suavemente até o formulário de atendimento ao pregoeiro ou abre a página de cotação)*.

### 2.3. Rodapé Institucional (Footer)
* **Fundo:** Azul Marinho Profundo (`#0A192F`) com textos em Branco Gelo (`#F8FAFC`) e cinza claro (`#94A3B8`).
* **Estrutura em 4 Colunas:**
  1. **Marca & Institucional:** Logo Ativa Brasil, breve descrição executiva, espaço reservado para Razão Social e CNPJ (`XX.XXX.XXX/0001-XX`), e selo de regularidade fiscal/cadastral (SICAF / Compras.gov.br).
  2. **Frente B2G (Órgãos Públicos):** Links rápidos para categorias de suprimentos, conformidade e envio de Termo de Referência.
  3. **Capacitação Estratégica:** Links para cursos, manuais e acesso direto ao Portal do Aluno (Hotmart).
  4. **Canais Oficiais:** E-mail corporativo (`contato@ativabrasilb2g.com.br`), WhatsApp Comercial B2G e cidade/estado de sede.

---

## 3. WIREFRAME DETALHADO DAS TELAS E SEÇÕES

### TELA 1: PÁGINA INICIAL (`index.html`)

#### Bloco 1.1: Hero Section (Abertura em Azul Marinho Profundo)
- **Estética:** Fundo Azul Marinho Profundo (`#0A192F`) em continuidade elegante à Splash Screen, com respiro generoso, tipografia editorial de alto contraste e movimento sutil de entrada. Layout assimétrico limpo (Texto à esquerda `60%` / Bloco Institucional de Autoridade à direita `40%`).
- **Conteúdo à Esquerda:**
  - *Badge Superior (Âmbar `#D97706` discreto):* `MESA DE OPERAÇÕES B2G & CAPACITAÇÃO ESTRATÉGICA`
  - *Headline (H1):* **Credibilidade institucional no fornecimento público e capacitação prática em dispensas eletrônicas.**
  - *Subheadline:* Atuação *asset-light* ágil junto a órgãos públicos e formação estratégica para quem deseja operar com segurança no mercado de compras governamentais.
  - *Dois Botões Lado a Lado:*
    - Primário (`#047857`): **Atendimento ao Pregoeiro / Cotação**
    - Secundário (Borda Clara): **Conhecer Cursos e Manuais**
- **Conteúdo à Direita (Bloco Institucional Executivo):**
  - Quadro sóbrio com transição suave destacando os 3 pilares de confiança:
    - ✓ **Conformidade & Idoneidade:** Estrutura alinhada à Lei 14.133/2021 e exigências do setor público.
    - ✓ **Operação Asset-Light:** Agilidade na resposta a demandas e foco em execução confiável.
    - ✓ **Visão Prática de Mercado:** Experiência real aplicada tanto ao atendimento B2G quanto à capacitação.

#### Bloco 1.2: Frente A — Áreas de Atuação Institucional (Sem Catálogo)
- **Fundo:** Branco Gelo (`#F8FAFC`).
- **Cabeçalho da Seção:** Título *"Áreas de Atuação no Fornecimento B2G"* + Subtítulo *"Atendimento institucional a dispensas de licitação e cotações, com foco em agilidade, conformidade e clareza operacional — sem catálogo de varejo."*
- **Apresentação Editorial:** Grade limpa e arejada com ícones lineares minimalistas e descrição institucional concisa das frentes de atuação (manutenção predial, suprimentos corporativos, equipamentos, segurança/EPIs, limpeza, informática e utilidades), acompanhada de fotografia corporativa/arquitetônica sóbria onde fizer sentido visual, sem fichas técnicas de produtos.
- **CTA da Seção:** Botão discreto *"Falar com a Mesa de Operações / Enviar Termo de Referência"*.

#### Bloco 1.3: Diferenciais Operacionais B2G (Faixa de Credibilidade)
* **Fundo:** Cinza Institucional Suave (`#F1F5F9`).
* **3 Pilares Horizontais:**
  1. **Agilidade na Resposta:** Orçamentos estruturados com rapidez e total aderência às especificações técnicas do Termo de Referência.
  2. **Rigor Documental:** Certidões negativas e habilitação jurídica mantidas rigorosamente em dia para contratação imediata.
  3. **Foco na Lei 14.133/2021:** Processos alinhados às exigências modernas de transparência e eficiência da Nova Lei de Licitações.

#### Bloco 1.4: Frente B — Capacitação Estratégica (Infoprodutos)
* **Fundo:** Branco Puro (`#FFFFFF`) com bordas de destaque.
* **Cabeçalho da Seção:**
  * *Tag:* `CAPACITAÇÃO ESTRATÉGICA`
  * *Título:* **Aprenda a vender para o governo começando do zero**
  * *Subtítulo:* Treinamentos práticos, manuais operacionais e mentorias baseados na rotina real de quem participa e vence dispensas eletrônicas todos os dias.
* **Vitrine de Produtos Digitais (Grid de 3 Cards Executivos):**
  * **Card 1 (E-book / Manual):** *Manual Prático da Dispensa Eletrônica* — Guia passo a passo do cadastro no SICAF à emissão da nota fiscal.
    * *Botões:* `Ver Ementa` (abre modal ou página de detalhes) | `Adquirir Agora` (link externo Hotmart).
  * **Card 2 (Curso Completo - Destaque com borda `#047857`):** *Formação Fornecedor B2G Asset-Light* — Método completo para estruturar sua operação de vendas ao governo sem precisar de estoque próprio.
    * *Botões:* `Ver Detalhes do Curso` | `Inscrever-se` (link externo Hotmart).
  * **Card 3 (Planilhas & Ferramentas / Mentoria):** *Kit Operacional & Precificação B2G* — Planilhas de formação de preço, cálculo de margem e checklists de habilitação.
    * *Botões:* `Conhecer Kit` | `Acessar Material` (link externo Hotmart).

#### Bloco 1.5: Canal Direto de Cotação B2G (Formulário Funcional)
* **Fundo:** Azul Marinho Profundo (`#0A192F`).
* **Layout:** 2 Colunas (À esquerda: orientações para servidores públicos/pregoeiros; À direita: formulário limpo em card branco).
* **Campos do Formulário:**
  * Nome do Responsável / Servidor
  * Órgão Público / Município / UF
  * E-mail Institucional (`.gov.br` ou oficial)
  * WhatsApp / Telefone de Contato
  * Número da Dispensa / Processo (Opcional)
  * Descrição resumida dos itens ou link do edital
* **Comportamento Técnico (Sem Backend):** Ao clicar em **"Enviar Solicitação de Cotação"**, o JavaScript valida os campos obrigatórios e oferece duas ações imediatas e confiáveis:
  1. Abre o WhatsApp Business da empresa já com a mensagem estruturada contendo todos os dados preenchidos pelo pregoeiro; E/OU
  2. Abre o cliente de e-mail (`mailto:`) pré-preenchido para envio formal. *(Exibe mensagem elegante de confirmação na tela).*

---

### TELA 2: PÁGINAS INTERNAS (OU SEÇÕES EXPANDIDAS)

* **Página/Modal de Detalhes do Produto Digital:**
  * Exibe título do treinamento, público-alvo, lista de módulos (acordeão expansível), garantia de 7 dias (padrão Hotmart) e botão grande em Verde Institucional (`#047857`) redirecionando para o checkout oficial da Hotmart.
* **Página Sobre Nós & Governança:**
  * Texto institucional focado em transparência, ética nas contratações públicas, eficiência logística e compromisso com o desenvolvimento do mercado B2G brasileiro.
* **Página de Contato:**
  * Cartões separados claramente:
    * **Canal 1: Setor de Licitações e Compras Públicas** (Foco em pregoeiros, envio de editais, notas de empenho e logística).
    * **Canal 2: Suporte ao Aluno e Capacitação** (Dúvidas sobre cursos, acesso à Hotmart e mentorias).

---

## 4. CONFIGURAÇÃO CENTRALIZADA DE LINKS (FACILIDADE DE MANUTENÇÃO)

Para facilitar futuras atualizações pelo proprietário do projeto (sem precisar caçar links espalhados pelo código), a IA deve criar um arquivo único de configuração (ex: `config.js` ou objeto de configuração no topo do script) contendo:
* `WHATSAPP_B2G`: Número oficial para cotações.
* `EMAIL_B2G`: E-mail oficial da empresa.
* `LINK_PORTAL_ALUNO`: URL da área de membros na Hotmart.
* `LINKS_CHECKOUT`: Objeto mapeando `produto_1`, `produto_2`, `produto_3` para suas respectivas URLs de checkout na Hotmart.