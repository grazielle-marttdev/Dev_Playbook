## Erro Comum: Pasta `components` Gigantesca

Um erro comum em projetos front-end é colocar todos os componentes da aplicação dentro de uma única pasta `components`.

Exemplo problemático:

```
src
 └── components
     ├── Header.jsx
     ├── Footer.jsx
     ├── ProductCard.jsx
     ├── LoginForm.jsx
     ├── UserProfile.jsx
     ├── CartItem.jsx
     └── ...
```

Conforme o projeto cresce, essa pasta pode se tornar difícil de navegar e manter.

### Problemas dessa abordagem

- Dificuldade para encontrar arquivos
- Componentes de funcionalidades diferentes misturados
- Aumento da complexidade conforme o projeto cresce

### Abordagem recomendada

Agrupar componentes por **funcionalidade** ou **contexto da aplicação**.

Exemplo:

```
src
 ├── features
 │   ├── auth
 │   │   └── components
 │   │       └── LoginForm.jsx
 │   │
 │   └── products
 │       └── components
 │           └── ProductCard.jsx
```

Isso mantém cada funcionalidade isolada e facilita a manutenção do projeto.