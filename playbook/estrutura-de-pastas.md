# Estrutura de Pastas

Este documento define a estrutura de pastas que utilizo em meus projetos front-end.  
O objetivo é manter o código organizado, previsível e fácil de manter.

---
--

## Visão Geral

| Pasta | Responsabilidade |
|------|------------------|
| src | Código fonte do projeto |
| css/base | Estilos globais |
| css/components | Estilos específicos de componentes |
| css/layout | Estrutura geral da página |
| css/utilities | Classes reutilizáveis |
| js/modules | Scripts separados por funcionalidade |
| components | Estruturas reutilizáveis da interface |
| assets | Arquivos estáticos como imagens e ícones |

---
--

## Estrutura do Projeto

```
project-name/
│
├── index.html
│
├── src/
│   │
│   ├── css/
│   │   ├── base/
│   │   │   ├── reset.css
│   │   │   └── globals.css
│   │   │
│   │   ├── components/
│   │   │   ├── header.css
│   │   │   ├── footer.css
│   │   │   ├── menu.css
│   │   │   └── card.css
│   │   │
│   │   ├── layout/
│   │   │   ├── container.css
│   │   │   └── sections.css
│   │   │
│   │   └── utilities/
│   │       ├── spacing.css
│   │       └── helpers.css
│   │
│   ├── js/
│   │   ├── main.js
│   │   └── modules/
│   │       └── menu.js
│   │
│   ├── components/
│   │   ├── header.html
│   │   ├── footer.html
│   │   └── card.html
│   │
│   └── assets/
│       ├── images/
│       └── icons/
│
└── README.md
```

---

## Princípios da Estrutura

### Separação de responsabilidades
Cada pasta possui uma função clara dentro do projeto.

### Organização por componentes
Componentes da interface possuem seus próprios estilos e, quando necessário, scripts específicos.

### Escalabilidade
A estrutura permite que o projeto cresça sem perder organização.

---

## Exemplo de Organização de um Componente

header.css

```css
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.header-nav {
  display: flex;
  gap: 20px;
}
```

Todos os estilos relacionados ao componente **header** ficam no mesmo arquivo.

---

### Regra geral:
Se um estilo pertence claramente a um componente, ele deve ficar em ```css/components```.