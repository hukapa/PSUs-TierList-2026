# ⚡ PSU Tier List (2025/2026) — Interactive Web Explorer

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Vanilla JS](https://img.shields.io/badge/Vanilla-JavaScript%20ES6+-F7DF1E?logo=javascript&logoColor=black)](#)
[![CSS3 Dark Mode](https://img.shields.io/badge/Design-Modern%20Dark%20Mode-0ea5e9)](#)
[![Zero Dependencies](https://img.shields.io/badge/Dependencies-Zero-emerald)](#)
[![GitHub Pages Ready](https://img.shields.io/badge/Deploy-GitHub%20Pages%20Ready-success)](#)

Uma aplicação web moderna, ultra-rápida e 100% autónoma para consultar, pesquisar e filtrar a consagrada **PSU Tier List** (base de dados técnica de fontes de alimentação para PC mantida pela comunidade **SPL - Single Pin Layout**).

Distribuição em **ficheiro único (`index.html`)** com zero dependências externas: funciona imediatamente com duplo clique offline (`file:///`) ou alojado gratuitamente no **GitHub Pages**.

---

## 🚀 Demonstração Rápida & Como Executar

### Opção 1: Execução Local Imediata (Offline)
1. Descarrega o ficheiro `index.html`.
2. Dá duplo clique no ficheiro para o abrir em qualquer browser moderno (Edge, Chrome, Brave, Firefox, Safari).
3. **Sem servidor local, sem Node.js, sem npm, sem erros de CORS.**

### Opção 2: Publicar Online via GitHub Pages (Grátis)
1. No teu repositório no GitHub, vai a **Settings** > **Pages** (no menu lateral).
2. Na secção **Build and deployment** > **Branch**:
   - Seleciona o branch `main` (ou `master`).
   - Mantém a pasta `/ (root)`.
3. Clica em **Save**.
4. Em cerca de 1 a 2 minutos, o teu projeto estará público e acessível em todo o mundo em:
   ```
   https://<o-teu-utilizador>.github.io/PSUs-TierList-2026/
   ```

---

## ✨ Funcionalidades Principais

* 🔍 **Pesquisa Multi-Termo Inteligente (Debounced):** Pesquisa combinada e simultânea por Marca, Série, Modelo, OEM ou Potência (ex: `"Toughpower PF3"`, `"RM850x"`, `"Focus Gold"`, `"HKC 1200W"`).
* 🏷️ **Filtro Rápido por Tier (Pills Alternáveis):** Seleciona um ou múltiplos Tiers ao mesmo tempo (ex: ver apenas Tier A e Tier B).
* ⚡ **Filtro de Norma ATX 3.0 / 3.1:** Interruptor acessível para isolar fontes compatíveis com a mais recente norma ATX 3.x e cabos 12V-2x6 / 12VHPWR.
* 🔋 **Filtro de Faixa de Potência:** Seletores imediatos para potências de entrada (`≤ 550W`, `600–750W`, `850–1000W`, `≥ 1050W`).
* 🥇 **Badges de Eficiência e Tier Padronizados:** Códigos de cores claros e imediatos para rápida identificação de risco/qualidade.
* 🗂️ **Gaveta Lateral de Ficha Técnica (*Drawer*):** Clica em qualquer linha para abrir todos os detalhes da fonte: fabricante OEM (CWT, Seasonic, HKC, Great Wall, etc.), código da plataforma interna, topologia (primária, retificação e regulação) e anotações técnicas completas da comunidade.
* 📋 **Copiar Ficha Técnica:** Botão para copiar instantaneamente um resumo estruturado da fonte para a área de transferência.
* 🔄 **Importação Dinâmica de CSV (Local FileReader):** Se o Google Sheets oficial for atualizado, basta arrastar o novo `.csv` para a aplicação para atualizar a base sem mexer no código.
* 📥 **Exportação de Dados:** Exporta os resultados filtrados diretamente para um novo ficheiro CSV limpo com suporte UTF-8.
* ⌨️ **Atalhos de Teclado:** <kbd>Ctrl</kbd> + <kbd>K</kbd> para focar na pesquisa, <kbd>Esc</kbd> para fechar gavetas e modais.

---

## 📊 Estrutura dos Tiers

| Tier | Classificação | Recomendação / Perfil | Cor do Badge |
| :---: | :--- | :--- | :---: |
| **A** | **Elite / Entusiasta** | Componentes de referência, baixíssimo ripple, regulação estrita e proteções completas. | 🟦 Azul Elétrico (`#38bdf8`) |
| **B** | **Mid-Range Superior** | Excelente relação qualidade/preço para builds de gaming de alto desempenho. | 🟨 Dourado (`#eab308`) |
| **C** | **Budget Recomendado** | Fontes económicas seguras para sistemas de consumo energético moderado. | 🟧 Laranja Suave (`#f97316`) |
| **D** | **Sistemas Integrados** | Apenas para sistemas muito básicos ou sem placa gráfica dedicada. | 🟫 Tijolo (`#fb923c`) |
| **E** | **Evitar** | Fontes com componentes de baixa durabilidade, ripple elevado ou proteções omissas. | 🟫 Tijolo Escuro (`#ea580c`) |
| **F** | **Perigo Crítico** | Risco comprovado de falha catastrófica, danos a componentes ou incêndio. | 🟥 Vermelho Alerta (`#ef4444`) |

---

## 🏆 Créditos Oficiais & Origem dos Dados

Todos os dados técnicos, testes laboratoriais, anotações de engenharia e classificações de modelos contidos nesta aplicação são fruto do esforço contínuo e altruísta de especialistas em hardware e da comunidade de entusiastas de PC.

### Fontes Oficiais:
* 📄 **Folha de Cálculo Oficial (Google Sheets):**  
  [SPL PSU Tier List — Google Sheets](https://docs.google.com/spreadsheets/d/1akCHL7Vhzk_EhrpIGkz8zTEvYfLDcaSpZRB6Xt6JWkc/htmlview#gid=1078495601)  
  *Mantida por **Sir ProvidenceLaw (SPL - Single Pin Layout)** e colaboradores da comunidade.*
* 🌐 **Website Oficial do Projeto:**  
  [psutierlist.org](https://psutierlist.org/)
* 🔬 **Laboratórios e Metodologia de Teste:**  
  * **Cybenetics Labs & Aris Mpitziopoulos ([Hardware Busters](https://hwbusters.com/)):** Medições profissionais em bancada de testes, osciloscópios, certificações ETA (eficiência) e LAMBDA (ruído).  
  * **Análises Independentes:** Desmontagens e testes elétricos detalhados realizados por analistas da TechPowerUp, Tom's Hardware, KitGuru e AnandTech.
* 🏛️ **Origem Histórica:**  
  O projeto dá continuidade ao legado construído pela equipa da *Cultists Network PSU Tier List* e pela comunidade original do *Linus Tech Tips Forum*.

---

## ⚖️ Aviso Legal & Isenção de Responsabilidade (Disclaimer)

1. **Projeto Independente e Não-Comercial:** Esta aplicação web é uma **ferramenta não-oficial de código aberto**, desenvolvida por iniciativa independente com o único propósito de proporcionar uma interface rápida, interativa e pesquisável para a comunidade de entusiastas de hardware.
2. **Sem Afiliação Formal:** Este projeto não é afiliado, patrocinado ou endossado pela equipa da SPL, pela Google, pelo Linus Tech Tips ou por qualquer um dos fabricantes de fontes de alimentação listados.
3. **Propriedade dos Dados:** As classificações, opiniões editoriais e anotações técnicas pertencem exclusivamente aos mantenedores da SPL PSU Tier List.
4. **Sem Garantias Implícitas:** As decisões de compra de hardware são da exclusiva responsabilidade do utilizador. Recomenda-se sempre a leitura das análises laboratoriais completas antes de efetuar qualquer aquisição.

---

## 📄 Licença

* O código-fonte da interface web (HTML, CSS e JavaScript) está licenciado sob a **[Licença MIT](LICENSE)**.
* Os dados técnicos de hardware e as classificações são disponibilizados publicamente pela comunidade SPL para benefício de todos os consumidores e construtores de PC.
