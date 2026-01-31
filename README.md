# 🚴 Bikcraft - Landing Page de Bicicletas Personalizadas

## 📋 Visão Geral do Projeto

Bikcraft é uma landing page moderna e elegante para uma empresa de bicicletas personalizadas. O projeto foi desenvolvido utilizando **HTML5**, **CSS3** e **SASS (SCSS)**, seguindo as melhores práticas de desenvolvimento web com design responsivo e animações suaves.

---

## 🏗️ Estrutura do Projeto

```
bikcraft/
├── 📄 index.html          # Página principal
├── 📄 contato.html        # Página de contato
├── 📄 produtos.html       # Página de produtos
├── 📄 portfolio.html      # Página de portfólio
├── 📄 sobre.html          # Página sobre a empresa
├── 📄 enviar.php          # Script de envio de formulários
├── 📁 css/
│   ├── 📄 style.css       # CSS compilado
│   └── 📁 scss/
│       ├── 📄 style.scss  # Arquivo principal do SASS
│       ├── 📄 _reset.scss # Reset CSS
│       ├── 📄 _normalize.scss # Normalização
│       ├── 📄 _grid.scss  # Sistema de grid
│       ├── 📄 _geral.scss # Estilos gerais
│       ├── 📄 _variaveis-e-mixins.scss # Variáveis e mixins
│       ├── 📄 _sobre.scss # Estilos da página sobre
│       ├── 📄 _produtos.scss # Estilos da página produtos
│       ├── 📄 _portfolio.scss # Estilos da página portfólio
│       └── 📄 _contato.scss # Estilos da página contato
├── 📁 img/
│   ├── 🖼️ bikcraft.png          # Logo
│   ├── 🖼️ bg.jpg                # Imagem de fundo
│   ├── 🖼️ bg-*.jpg              # Imagens de fundo específicas
│   ├── 📁 produtos/
│   │   ├── 🚲 passeio.png       # Ícone bicicleta Passeio
│   │   ├── 🚲 esporte.png       # Ícone bicicleta Esporte
│   │   └── 🚲 retro.png         # Ícone bicicleta Retrô
│   ├── 📁 portfolio/
│   │   ├── 🏞️ retro.jpg
│   │   ├── 🏞️ passeio.jpg
│   │   └── 🏞️ esporte.jpg
│   └── 📁 redes-sociais/
│       ├── 📘 facebook.png
│       ├── 📸 instagram.png
│       └── 🐦 twitter.png
└── 📁 js/
    ├── 📜 main.js        # Scripts principais
    ├── 📜 plugins.js     # Plugins jQuery
    └── 📁 libs/
        ├── 📦 jquery-1.11.2.min.js
        └── 📦 modernizr.custom.45655.js
```

---

## 🎨 Tecnologias Utilizadas

| Tecnologia           | Descrição                                                      |
| -------------------- | -------------------------------------------------------------- |
| 🟦 **HTML5**         | Linguagem de marcação semântica com meta tags SEO e Open Graph |
| 🎨 **CSS3**          | Estilização com transições, animações e design responsivo      |
| 🟨 **SASS/SCSS**     | Pré-processador CSS com variáveis, mixins e modularidade       |
| 📜 **jQuery 1.11.2** | Biblioteca JavaScript para interações e animações              |
| ⚡ **Modernizr**     | Detecção de recursos HTML5/CSS3                                |

---

## 📱 Estrutura HTML

### 🌐 Cabeçalho (Header)

```html
<header class="header">
  <div class="container">
    <a href="index.html" class="grid-4">
      <img src="img/bikcraft.png" alt="Bikcraft" />
    </a>
    <nav class="grid-12 header_menu">
      <ul>
        <li><a href="sobre.html">Sobre</a></li>
        <li><a href="produtos.html">Produtos</a></li>
        <li><a href="portfolio.html">Portfólio</a></li>
        <li><a href="contato.html">Contato</a></li>
      </ul>
    </nav>
  </div>
</header>
```

### 🏠 Seção Introdução

```html
<section class="introducao">
  <div class="container">
    <h1>Bicicletas Feitas a Mão</h1>
    <blockquote class="quote-externo">
      <p>
        "não tenha nada em sua casa que você não considera útil ou acredita ser
        bonito"
      </p>
      <cite>WILLIAM MORRIS</cite>
    </blockquote>
    <a href="produtos.html" class="btn">Orçamento</a>
  </div>
</section>
```

---

## 🎯 Principais Seções

### 🚲 Produtos (3 Categorias)

| Categoria   | Descrição                   | Ícone |
| ----------- | --------------------------- | ----- |
| **Passeio** | Conforto para seus passeios | 🛤️    |
| **Esporte** | Performance e velocidade    | ⚡    |
| **Retró**   | Estilo clássico atemporal   | ⏰    |

### 📊 Qualidade

Diferenciais da Bikcraft:

- 💪 **Durabilidade** - Sólida como pedra, leve como o vento
- 🎨 **Design** - Feitas sob medida para seu conforto
- 🌱 **Sustentabilidade** - Produção ecológica e sustentável

### 📞 Footer

Contém:

- 📖 **Nossa História** - A trajetória da Bikcraft
- 📞 **Contatos** - Telefone, email e localização
- 🌐 **Redes Sociais** - Facebook, Instagram e Twitter

---

## 🎨 Sistema de Cores

```scss
$amarelo: #fec63e; // Cor primária (amarelo)
$black: #000000; // Preto
$white: #ffffff; // Branco
```

---

## 📐 Sistema de Grid

O projeto utiliza um sistema de grid responsivo com as seguintes classes:

- `grid-1-3` - 1/3 da largura
- `grid-4` - 4/16 da largura (25%)
- `grid-8` - 8/16 da largura (50%)
- `grid-16` - 16/16 da largura (100%)

---

## ✨ Recursos Especiais

### 🔄 Animações

```scss
// FadeInDown Animation
@keyframes fadeInDown {
  0% {
    opacity: 0;
    transform: translate3d(0, -20px, 0);
  }
  100% {
    opacity: 1;
    transform: none;
  }
}
```

### 📱 Design Responsivo

Breakpoints definidos via mixins SASS:

- `d(t)` - Tablet
- `d(m)` - Mobile

### 🧩 Mixins SASS

```scss
// Mixin para tipografia
@mixin tipo-1($size) {
  font-size: $size + px;
  // ... mais estilos
}

// Mixin para breakpoints
@mixin d($device) {
  @if $device == t {
    @media only screen and (max-width: 767px) {
      @content;
    }
  }
}
```

---

## 🖼️ Ícones do Projeto

O projeto utiliza ícones nas seguintes áreas:

| Localização          | Ícones                                         |
| -------------------- | ---------------------------------------------- |
| 🏷️ **Logo**          | `bikcraft.png`                                 |
| 🚲 **Produtos**      | `passeio.png`, `esporte.png`, `retro.png`      |
| 📱 **Redes Sociais** | `facebook.png`, `instagram.png`, `twitter.png` |

---

## 📈 SEO e Meta Tags

O projeto inclui meta tags otimizadas para SEO:

```html
<meta
  name="description"
  content="Compre a sua bicicleta personalizada na Bikcraft..."
/>
<meta property="og:type" content="website" />
<meta property="og:title" content="Bikcraft - Bicicletas Personalizadas" />
<meta property="og:description" content="..." />
<meta property="og:image" content="http://bikcraft.com/img/og-image.png" />
```

---

## 🚀 Como Executar

1. **Clone o repositório:**

   ```bash
   git clone https://github.com/seu-repositorio/bikcraft.git
   ```

2. **Abra no navegador:**

   ```bash
   # Abra o arquivo index.html diretamente
   firefox index.html
   # ou
   google-chrome index.html
   ```

3. **Para desenvolvimento SASS:**

   ```bash
   # Instale o SASS globalmente
   npm install -g sass

   # Compile o SASS
   sass css/scss/style.scss css/style.css --watch
   ```

---

## 📝 Conclusão

A **Bikcraft** é uma landing page completa que demonstra:

- ✅ **HTML Semântico** - Estrutura bem organizada e acessível
- ✅ **CSS Moderno** - Flexbox, animações e design responsivo
- ✅ **SASS Avançado** - Variáveis, mixins e modularidade
- ✅ **UX/UI** - Design intuitivo e visual atraente
- ✅ **SEO** - Meta tags otimizadas para busca
- ✅ **Performance** - Imagens otimizadas e código eficiente

Este projeto serve como excelente referência para quem deseja aprender desenvolvimento web moderno com **HTML, CSS e SASS**.

---

> 🏆 _Bikcraft - Bicicletras Feitas a Mão com Amor e Arte_
