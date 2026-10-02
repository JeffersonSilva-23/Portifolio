# Portfólio Web — Jefferson Honório

> Portfólio pessoal desenvolvido como primeiro projeto prático de desenvolvimento web, aplicando HTML5 semântico, CSS Grid, Flexbox e responsividade.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/docs/Web/CSS)
[![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)](https://git-scm.com)
[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-222?style=flat-square&logo=github)](https://pages.github.com)
[![Status](https://img.shields.io/badge/status-conclu%C3%ADdo-success?style=flat-square)](#)

---

## Sumário

- [Sobre o Projeto](#sobre-o-projeto)
- [Demonstração](#demonstração)
- [Técnicas e Estruturas Utilizadas](#técnicas-e-estruturas-utilizadas)
- [Tecnologias](#tecnologias)
- [Estrutura de Arquivos](#estrutura-de-arquivos)
- [Como Executar o Projeto](#como-executar-o-projeto)
- [Próximos Passos](#próximos-passos)
- [Autor](#autor)
- [Licença](#licença)

---

## Sobre o Projeto

Este repositório reúne o código do meu primeiro portfólio web, criado com o objetivo de colocar em prática os fundamentos do desenvolvimento front-end. O projeto foi estruturado para servir como base de estudos e, ao mesmo tempo, apresentar de forma organizada minha trajetória, projetos e habilidades técnicas.

A proposta foi construir uma página única (single page), leve e responsiva, sem dependência de frameworks, priorizando:

- **Semântica correta** do HTML5 para acessibilidade e SEO.
- **CSS puro** com Grid Layout e Flexbox para um layout moderno.
- **Responsividade mobile-first** para leitura confortável em qualquer dispositivo.
- **Versionamento com Git** e publicação contínua via GitHub Pages.

---

## Demonstração

🔗 **Acesse online:** [https://jeffersonsilva-23.github.io](https://jeffersonsilva-23.github.io)

> Substitua o link acima pela URL real do deploy, caso já esteja publicado no GitHub Pages.

---

## Técnicas e Estruturas Utilizadas

### HTML5 Semântico

Uso das tags estruturais corretas para organizar o conteúdo de forma compreensível tanto para navegadores quanto para leitores de tela e mecanismos de busca:

```html
<header>  <!-- Cabeçalho com logotipo e navegação -->
<nav>     <!-- Menu principal -->
<main>    <!-- Conteúdo principal -->
<section> <!-- Blocos temáticos: sobre, projetos, habilidades, formação -->
<footer>  <!-- Rodapé com contato e direitos autorais -->
```

### CSS Grid Layout

O layout principal é estruturado com `grid-template-areas`, mapeando visualmente a posição de cada bloco da página:

```css
.container {
  display: grid;
  grid-template-areas:
    "header"
    "hero"
    "sobre"
    "projetos"
    "habilidades"
    "formacao"
    "footer";
  gap: 2rem;
}
```

### Flexbox

Aplicado em listas dinâmicas (`.habilidades-devs`, `.timeline-cursos`) para permitir alinhamento flexível e quebra automática de linha:

```css
.habilidades-devs {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}
```

### Media Queries

Responsividade implementada com breakpoint em `768px`, reorganizando o Grid para uma coluna única em dispositivos móveis:

```css
@media (max-width: 768px) {
  .container {
    grid-template-areas:
      "header"
      "hero"
      "sobre"
      /* ... */
      "footer";
    grid-template-columns: 1fr;
  }
}
```

### Versionamento com Git

Histórico de commits organizado com mensagens descritivas e publicação via GitHub Pages.

---

## Tecnologias

| Tecnologia | Propósito |
|------------|-----------|
| **HTML5** | Estruturação semântica do conteúdo |
| **CSS3** | Estilização, layout (Grid + Flexbox) e responsividade |
| **Git** | Controle de versão local |
| **GitHub** | Hospedagem do repositório e deploy via Pages |
| **VS Code** | Editor de código |

---

## Estrutura de Arquivos

```
portfolio/
├── index.html          # Página principal
├── css/
│   └── style.css       # Folha de estilos
├── assets/
│   └── foto.jpg        # Foto de perfil
└── README.md           # Este arquivo
```

---

## Como Executar o Projeto

### Pré-requisitos

Nenhuma instalação é necessária além de um navegador web moderno. Para clonar o repositório, é preciso ter o **Git** instalado.

### Passo a passo

1. Clone o repositório:

   ```bash
   git clone https://github.com/JeffersonSilva-23/portfolio.git
   ```

2. Acesse a pasta do projeto:

   ```bash
   cd portfolio
   ```

3. Abra o arquivo `index.html` diretamente no navegador.

   - **Opção A:** clique duas vezes no arquivo.
   - **Opção B:** use a extensão **Live Server** no VS Code para recarregamento automático.

---

## Próximos Passos

Melhorias planejadas para as próximas versões:

- [ ] Migrar para variáveis CSS (design tokens) para facilitar manutenção de tema
- [ ] Adicionar modo claro/escuro com `prefers-color-scheme`
- [ ] Implementar acessibilidade completa (WCAG 2.2 AA)
- [ ] Incluir animações de entrada com `IntersectionObserver`
- [ ] Adicionar formulário de contato funcional
- [ ] Otimizar imagens (formato WebP + `loading="lazy"`)
- [ ] Publicar com domínio próprio

---

## Autor

**Jefferson Honório da Silva**

Desenvolvedor full stack em formação — Técnico em Desenvolvimento de Sistemas (SENAI Maracanã).

[![GitHub](https://img.shields.io/badge/GitHub-JeffersonSilva--23-181717?style=flat-square&logo=github)](https://github.com/JeffersonSilva-23)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-jefferson--honorio--dev-0A66C2?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/jefferson-honorio-dev/)
[![E-mail](https://img.shields.io/badge/E--mail-honoriojefferson45%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:honoriojefferson45@gmail.com)

---

## Licença

Este projeto está sob a licença **MIT**. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.

```
MIT License

Copyright (c) 2026 Jefferson Honório da Silva

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

<p align="center">
  Feito com dedicação por <a href="https://github.com/JeffersonSilva-23">Jefferson Honório</a>
</p>