# Estrutura de Pastas (Projetos React)

Esta estrutura é utilizada em projetos front-end maiores que utilizam React e ferramentas modernas de build como Vite.

O objetivo é manter o código modular, escalável e fácil de manter conforme o projeto cresce.

---

## Visão Geral

| Pasta | Responsabilidade |
|------|------------------|
| assets | Arquivos estáticos (imagens, ícones, fontes) |
| components | Componentes reutilizáveis da interface |
| pages | Páginas principais da aplicação |
| layouts | Estruturas de layout reutilizáveis |
| hooks | Hooks personalizados |
| services | Comunicação com APIs |
| utils | Funções auxiliares reutilizáveis |
| styles | Estilos globais |

---

## Estrutura do Projeto

```
project-name/
│
├── public/
│
├── src/
│   │
│   ├── assets/
│   │   ├── images/
│   │   └── icons/
│   │
│   ├── components/
│   │   ├── Header/
│   │   │   ├── Header.jsx
│   │   │   └── header.css
│   │   │
│   │   └── Card/
│   │       ├── Card.jsx
│   │       └── card.css
│   │
│   ├── pages/
│   │   ├── Home/
│   │   │   └── Home.jsx
│   │   │
│   │   └── About/
│   │       └── About.jsx
│   │
│   ├── layouts/
│   │   └── MainLayout.jsx
│   │
│   ├── hooks/
│   │   └── useMenu.js
│   │
│   ├── services/
│   │   └── api.js
│   │
│   ├── utils/
│   │   └── formatDate.js
│   │
│   ├── styles/
│   │   └── global.css
│   │
│   ├── App.jsx
│   └── main.jsx
│
├── package.json
└── README.md
```

---

## Princípios dessa Estrutura

### Componentização
Cada componente possui sua própria pasta, contendo:

- o componente
- seus estilos
- arquivos relacionados

Isso facilita manutenção e reutilização.

---

### Separação entre interface e lógica

- **components** → elementos reutilizáveis da interface  
- **pages** → páginas completas da aplicação  
- **services** → comunicação com APIs  
- **utils** → funções auxiliares  

---

### Escalabilidade

Essa organização permite que o projeto cresça sem transformar o diretório `src` em um local confuso.

---

## Regra Geral

Se um arquivo pertence claramente a um componente, ele deve ficar dentro da pasta desse componente.