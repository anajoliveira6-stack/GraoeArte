# Grão & Arte - Torrefação e Café Especial ☕

> Projeto desenvolvido como simulação de front-end profissional para a disciplina/curso do SENAI Henrique Lupo, aplicando conceitos de semântica HTML5, arquitetura CSS modular (BEM), acessibilidade, responsividade e escalas relativas.

---

## 📋 Sumário
- [Visão Geral](#-visão-geral)
- [Tecnologias e Conceitos Aplicados](#-tecnologias-e-conceitos-aplicados)
- [Organização da Arquitetura de Arquivos](#-organização-da-arquitetura-de-arquivos)
- [Instruções de Visualização e Execução](#-instruções-de-visualização-e-execução)
- [Requisitos do Projeto](#-requisitos-do-projeto)
- [Principais Desafios Técnicos e Aprendizados](#-principais-desafios-técnicos-e-aprendizados)
- [Licença e Créditos](#-licença-e-créditos)

---

## ☕ Visão Geral

O projeto **Grão & Arte** é uma landing page responsiva e interativa desenvolvida para uma torrefação artesanal de cafés especiais. O público-alvo compreende apreciadores de cafés especiais, métodos de extração artesanais e assinantes de grãos selecionados (100% Arábica, com pontuação superior a 85 pontos SCA).

A aplicação foi planejada do zero com foco em autonomia de layout, semântica, experiência do usuário (UX/UI) e boas práticas de código front-end.

---

## 🛠️ Tecnologias e Conceitos Aplicados

* **HTML5 Semântico**: Estruturação limpa com tags adequadas (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<details>`, `<summary>`, `<footer>`) sem o uso de estilos inline.
* **CSS3 & CSS Variables (Design System)**: Uso de tokens de design para cores, fontes e sombras organizados via `:root`.
* **Metodologia BEM (Block Element Modifier)**: Padronização de classes no HTML e seletores no CSS para garantir legibilidade e reaproveitamento do código.
* **Tipografia e Escala REM**:
  * Ajuste da escala da fonte base no elemento raiz (`html`).
  * Resgate do tamanho padrão no `body`.
  * Toda tipografia, espaçamentos e bordas definidos estritamente em unidades relativas (`rem`).
* **Unidades de Layout Flexíveis**:
  * Utilização de `%` para larguras de containers flexíveis.
  * Uso de `vh` e `vw` para controle de altura de seções em tela cheia.
  * Restrições rígidas quanto ao uso de pixels (apenas para bordas e detalhes específicos).
* **Flexbox**: Utilizado na construção da distribuição dos elementos, cards e menus de navegação.
* **Google Fonts**: Importação das famílias `Merriweather` (pesos 400 e 700) e `Open Sans` (pesos 400, 600 e 700).
* **Responsividade**: Layout adaptável estruturado via *media queries* e pontos de quebra (*breakpoints*) estratégicos para smartphones, tablets e desktops.

---

## 📂 Organização da Arquitetura de Arquivos

A estrutura do projeto adota a separação de responsabilidades recomendada no RNF04:

```text
grao-e-arte/
├── assets/
│   ├── css/
│   │   ├── variables.css      # Variáveis globais do Design System (:root)
│   │   ├── reset.css          # Normalização e escala de fontes base (REM)
│   │   ├── components.css     # Estilização de componentes e metodologia BEM
│   │   ├── layout.css         # Estrutura de seções, Flexbox e media queries
│   │   └── style.css          # Arquivo principal que importa as demais folhas
│   └── images/                # Imagens locais ou assets visuais
├── index.html                 # Estrutura principal em HTML5 semântico
└── README.md                  # Documentação do projeto