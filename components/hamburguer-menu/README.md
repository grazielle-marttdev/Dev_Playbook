# Hamburger Menu (Acessível)

Criar um menu hambúrguer acessível e fácil de reutilizar.

## Princípios

- Estado controlado com `aria-expanded`
- Botão com `aria-controls`
- Navegação funcional com teclado
- Estrutura semântica

## Estrutura HTML

```html
<body>
    <button id="menu-toggle-btn" aria-label="Abrir menu" aria-expanded="false" aria-controls="menu">
        <i class="fa-solid fa-bars"></i>
    </button>

    <nav class="active" id="menu">
        <ul>
            <li>Sobre</li>
            <li>Projetos</li>
            <li>Contato</li>
        </ul>
    </nav>

    <script src="script.js"></script>
</body>
```

## Lógica JavaScript

```js
const btnMenu = document.getElementById('menu-toggle-btn')
const menu = document.getElementById('menu')

btnMenu.addEventListener('click', () => {
    const isExpanded = btnMenu.getAttribute('aria-expanded') === 'true'

    btnMenu.setAttribute('aria-expanded', !isExpanded)
    menu.classList.toggle('active')
});
```

## Observações

- Evitar depender apenas de classes para estado
- Garantir foco acessível