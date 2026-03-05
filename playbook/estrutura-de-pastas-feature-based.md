# Estrutura de Pastas (Feature-Based Architecture)

Esta arquitetura organiza o projeto por funcionalidades (features) em vez de separar arquivos apenas por tipo.

O objetivo é tornar projetos grandes mais organizados, previsíveis e escaláveis.

---

## Estrutura do Projeto

```
project-name/
│
├── public/
│
├── src/
│
│   ├── assets/
│   │   ├── images/
│   │   └── icons/
│   │
│   ├── features/
│   │
│   │   ├── auth/
│   │   │   ├── components/
│   │   │   │   └── LoginForm.jsx
│   │   │   │
│   │   │   ├── hooks/
│   │   │   │   └── useAuth.js
│   │   │   │
│   │   │   ├── services/
│   │   │   │   └── authService.js
│   │   │   │
│   │   │   └── pages/
│   │   │       └── LoginPage.jsx
│   │   │
│   │   ├── products/
│   │   │   ├── components/
│   │   │   │   └── ProductCard.jsx
│   │   │   │
│   │   │   ├── services/
│   │   │   │   └── productService.js
│   │   │   │
│   │   │   └── pages/
│   │   │       └── ProductsPage.jsx
│   │
│   ├── shared/
│   │   ├── components/
│   │   │   └── Button.jsx
│   │   │
│   │   ├── hooks/
│   │   │   └── useFetch.js
│   │   │
│   │   └── utils/
│   │       └── formatCurrency.js
│   │
│   ├── layouts/
│   │   └── MainLayout.jsx
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

## Conceito de Feature

Uma **feature** representa uma funcionalidade completa da aplicação.

Exemplos:

- autenticação
- carrinho de compras
- perfil do usuário
- listagem de produtos

Cada feature contém tudo que precisa para funcionar.

---

## Pasta `features`

Cada pasta representa uma funcionalidade da aplicação.

Exemplo:

```
features
 ├── auth
 └── products
```

Isso evita que o código da aplicação fique espalhado por muitas pastas diferentes.

---

## Pasta `shared`

Contém código reutilizável por várias features.

Exemplos:

- botões
- hooks genéricos
- funções utilitárias

---

## Vantagens dessa Arquitetura

- Melhor organização em projetos grandes
- Funcionalidades isoladas
- Mais fácil escalar o projeto
- Facilita trabalho em equipe

---

## Regra Geral

Se o código pertence a uma funcionalidade específica, ele deve ficar dentro da pasta dessa feature.