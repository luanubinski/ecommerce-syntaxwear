# Syntaxwear - E-commerce de Tênis e Sneakers

![Syntaxwear Logo](./images/logo/logo.svg)

Syntaxwear é uma plataforma de e-commerce moderna e responsiva especializada na venda de tênis e sneakers online. O site oferece uma experiência de compra intuitiva com design contemporâneo e navegação otimizada para todos os dispositivos.

## 📋 Características

- **Design Responsivo**: Otimizado para desktop, tablet e mobile
- **Menu Hamburger**: Navegação adaptativa para dispositivos móveis
- **Seção Hero**: Banner destacado com call-to-action
- **Categorias de Produtos**: Casual, Esporte, Moderno e Futurista
- **Grid de Produtos**: Layout dinâmico com cards em diferentes tamanhos
- **Newsletter**: Formulário de inscrição integrado no rodapé
- **Redes Sociais**: Links para Instagram, WhatsApp, TikTok e Facebook
- **Acessibilidade**: Uso de labels, aria-labels e semântica HTML5

## 🗂️ Estrutura do Projeto

```
ecommerce-syntaxwear/
├── index.html                 # Arquivo principal da aplicação
├── README.md                  # Este arquivo
├── css/
│   ├── reset.css             # Reset CSS (Andy Bell's Modern CSS Reset)
│   ├── variables.css         # Variáveis CSS e fonts
│   ├── base.css              # Estilos base e componentes reutilizáveis
│   └── components/           # Estilos dos componentes específicos
│       ├── header.css        # Estilos do header e navegação
│       ├── hero.css          # Estilos da seção hero
│       ├── product-category.css  # Estilos dos cards de categoria
│       ├── product-grid.css  # Estilos do grid de produtos
│       └── footer.css        # Estilos do rodapé
└── images/
    ├── logo/
    │   └── logo.svg          # Logo da marca
    ├── icons/                # Ícones SVG
    │   ├── hamburguer.svg    # Ícone do menu mobile
    │   ├── user.svg          # Ícone de usuário
    │   ├── help.svg          # Ícone de ajuda
    │   ├── bag.svg           # Ícone de carrinho
    │   ├── instagram.svg     # Ícone Instagram
    │   ├── whatsapp.svg      # Ícone WhatsApp
    │   ├── tiktok.svg        # Ícone TikTok
    │   └── facebook.svg      # Ícone Facebook
    ├── banners/              # Imagens dos banners
    ├── products/             # Imagens dos produtos
    └── favicons/             # Favicons do site
```

## 🎨 Arquitetura CSS

O projeto utiliza uma arquitetura CSS escalável e bem organizada:

### 1. **reset.css**
   - Reset moderno baseado no método de Andy Bell
   - Remove estilos padrão do navegador
   - Define comportamentos base (box-sizing, scroll suave, etc.)

### 2. **variables.css**
   - Define a fonte principal: Ubuntu (do Google Fonts)
   - Ponto central para variáveis CSS globais

### 3. **base.css**
   - Estilos base da aplicação
   - Classes reutilizáveis (.btn, .btn-outline, .btn-filled)
   - Layout responsivo (main container com max-width 1360px)
   - Efeitos hover nos botões

### 4. **components/**
   - **header.css**: Navegação, logo, menu hamburger
   - **hero.css**: Seção banner destacada com overlay
   - **product-category.css**: Cards das categorias
   - **product-grid.css**: Grid masonry de produtos
   - **footer.css**: Rodapé com links e newsletter

## 🎯 Seções Principais

### Header
- Logo/Branding
- Navegação Principal (Masculino, Feminino, Outlet)
- Navegação Secundária (Lojas, Sobre, Conta, Ajuda, Carrinho)
- Menu responsivo para mobile

### Hero Section
- Banner com imagem de fundo
- Overlay escuro
- Título e subtítulo
- Dois botões CTA (Outline e Filled)

### Categorias de Produtos
4 cards com hover effect:
- **Casual**: Para o dia a dia
- **Esporte**: Para atividades físicas
- **Moderno**: Estilo contemporâneo
- **Futurista**: Design inovador

### Grid de Produtos
Layout masonry com:
- 1 card grande (top1) - Destaque Krypto One
- 2 cards de tamanho normal (top2, midL, midR)
- 2 cards pequenos (bottomL, bottomR)

### Footer
- **Newsletter**: Formulário de inscrição por email
- **Redes Sociais**: Links para redes com ícones
- **Navegação**: Links organizados por categoria
  - Masculino / Feminino / Outlet / Lojas / Sobre
- **Rodapé**: Copyright e créditos

## 🔌 Links de CSS no HTML

O `index.html` carrega os arquivos CSS na seguinte ordem:

```html
<link rel="stylesheet" href="/css/reset.css" />
<link rel="stylesheet" href="/css/variables.css" />
<link rel="stylesheet" href="/css/base.css" />
<link rel="stylesheet" href="/css/layout.css" />
<link rel="stylesheet" href="./css/components/header.css" />
<link rel="stylesheet" href="./css/components/hero.css" />
<link rel="stylesheet" href="./css/components/product-category.css" />
<link rel="stylesheet" href="./css/components/product-grid.css" />
<link rel="stylesheet" href="./css/components/footer.css" />
```

## 🎨 Design System

### Tipografia
- **Fonte Principal**: Ubuntu (peso: 300, 400, 500, 700)
- Importada do Google Fonts

### Paleta de Cores
- **Principal**: `#6329a2` (Roxo)
- **Texto**: `#333333` (Cinza escuro)
- **Fundo**: `#ffffff` (Branco)
- **Bordas**: `#ffffff` (Branco para contraste)

### Componentes de Botão
```css
.btn              /* Classe base */
.btn-outline      /* Botão com borda (transparente) */
.btn-filled       /* Botão preenchido (roxo/branco) */
```

**Efeito Hover**: Fundo roxo (#6329a2) com texto branco

## 📱 Responsividade

O site é otimizado para diferentes tamanhos de tela:

- **Desktop**: Layout completo com navegação horizontal
- **Tablet**: Navegação adaptada (max-width: 1280px)
- **Mobile**: Menu hamburger, layout em coluna única

## 🔗 Links de Navegação

### Categorias Masculino
- Casual, Esporte, Moderno, Futurista

### Categorias Feminino
- Casual, Esporte, Moderno, Futurista

### Outlet
- Masculino, Feminino

### Nossas Lojas
- Loja Física, Loja Online

### Sobre
- Quem Somos, Missão

## 🚀 Próximos Passos

- Implementar lógica JavaScript para o menu mobile
- Integrar banco de dados para produtos
- Implementar funcionalidade de carrinho
- Adicionar página de detalhes do produto
- Integrar gateway de pagamento
- Adicionar autenticação de usuário

---

**Syntaxwear** - Transforme qualquer passo em presença! 👟