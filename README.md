# 📺 Desafio DIO: Reproduzindo a Listagem do YouTube com CSS Grid Layout

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![CSS Grid](https://img.shields.io/badge/Layout-CSS_Grid-2965f1?style=for-the-badge&logo=css3&logoColor=white)
![Flexbox](https://img.shields.io/badge/Layout-Flexbox-00C4CC?style=for-the-badge&logo=css3&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge)

</div>

Projeto prático desenvolvido para o desafio **"Reproduzindo a listagem do YouTube com Grid Layout no CSS"**, pertencente à **Trilha CSS Web Developer** da [DIO (Digital Innovation One)](https://www.dio.me/), sob orientação da expert **Michele Ambrosio**.

---

## 📌 Visão Geral do Projeto

Neste projeto prático, reproduzimos a interface da tela inicial (Home Feed / Listagem de Vídeos) do **YouTube**, explorando todo o poder e flexibilidade do **CSS Grid Layout** em conjunto com **Flexbox** para componentes internos e alinhamentos de navegação.

O projeto foi construído fielmente às especificações do protótipo oficial do **Figma**, assegurando fidelidade visual, estruturação semântica, microinterações e alta responsividade.

---

## 🚀 Funcionalidades & Componentes

- **Header Fixo (Sticky Navbar):**
  - Botão de acionamento do menu hambúrguer e logotipo oficial do YouTube.
  - Campo de busca centralizado com efeito de foco, botão de lupa e acionamento por voz (microfone).
  - Ações rápidas do usuário: criar conteúdo, notificações e foto de perfil.

- **Barra Lateral de Navegação (Sidebar):**
  - Menus categorizados:
    - Principal: *Início (ativo)*, *Explorar*, *Inscrições*.
    - Biblioteca pessoal: *Biblioteca*, *Histórico*, *Assistir mais tarde*, *Vídeos com gostei*.
    - Canais inscritos: Canal *DIO* com avatar e badge.
  - Comportamento responsivo (colapsa em ícones ou oculta em telas menores).

- **Barra de Chips / Filtros de Categorias:**
  - Carrossel horizontal de filtros rápidos (*Tudo*, *Programação*, *Ciência de Dados*, *CSS Grid*, etc.).

- **Grade Principal de Vídeos (CSS Grid):**
  - Cards de vídeos estruturados em grid fluido com `auto-fill` e `minmax(280px, 1fr)`.
  - Miniaturas com proporção `16:9` (`aspect-ratio: 16 / 9`) e efeito de zoom suave ao passar o cursor (*hover*).
  - Selo de tempo de duração sobreposto à miniatura.
  - Avatar do canal, título com corte de linha elíptico em 2 linhas (`-webkit-line-clamp: 2`), nome do canal com selo de verificação e métricas de visualizações/tempo decorrido.

---

## 📐 Conceitos e Propriedades de CSS Grid Aplicados

| Propriedade CSS Grid | Aplicação no Projeto |
| :--- | :--- |
| `display: grid` | Habilitação do contexto de grid bidimensional na seção `.video-grid` |
| `grid-template-columns: repeat(auto-fill, minmax(280px, 1fr))` | Responsividade automática: calcula a quantidade de colunas conforme o espaço disponível na tela |
| `gap: 28px 16px` | Espaçamento uniforme entre as linhas (28px) e colunas (16px) de vídeos |
| `minmax(280px, 1fr)` | Garante que cada card tenha no mínimo 280px de largura e expanda igualmente para preencher o container |
| `aspect-ratio: 16 / 9` | Proporção matemática perfeita para as miniaturas de vídeo sem deformação |

---

## 📁 Estrutura de Pastas

```text
desafio7/
├── assets/
│   ├── css/
│   │   └── styles.css          # Estilização completa (CSS Grid & Flexbox)
│   └── img/
│       ├── dio.png             # Avatar do canal DIO
│       ├── icon-youtube.png    # Favicon oficial
│       ├── logo-youtube.png    # Logotipo do YouTube
│       ├── photo-user.jpg      # Foto de perfil do usuário
│       └── thumbnails/         # Miniaturas dos vídeos da grade
│           ├── thumbnail-01.png
│           ├── thumbnail-02.png
│           ├── thumbnail-03.png
│           ├── thumbnail-04.png
│           └── thumbnail-05.png
├── index.html                  # Estrutura semântica HTML5
├── README.md                   # Documentação detalhada
└── .gitignore                  # Arquivos ignorados pelo controle de versão
```

---

## 🛠️ Como Executar Localmente

1. Clone o repositório:
   ```bash
   git clone https://github.com/MatheusMittz/trilha-css-desafio-03.git
   ```
2. Entre na pasta:
   ```bash
   cd trilha-css-desafio-03
   ```
3. Abra o arquivo `index.html` em qualquer navegador web (ou utilize a extensão **Live Server** no VS Code).

---

## 🔗 Referências

- [Trilha CSS Developer na DIO](https://web.dio.me/track/formacao-css-web-developer)
- [Desafio de Projeto DIO: Reproduzindo a listagem do YouTube com Grid Layout no CSS](https://web.dio.me/project/reproduzindo-a-listagem-do-youtube-com-grid-layout-no-css-grid-figma/learning/f4d586be-80c8-4aa1-9fb9-b1cce284bdd6?back=/track/formacao-css-web-developer)

---

## 👤 Autor

Desenvolvido por **[Matheus Mittz](https://github.com/MatheusMittz)**.
