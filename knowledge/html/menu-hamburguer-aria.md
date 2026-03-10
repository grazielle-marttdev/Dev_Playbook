## Menu hambúrguer — controle de estado

Menus hambúrguer devem expor seu estado de abertura para melhorar acessibilidade e clareza de implementação.

A forma recomendada é usar o atributo `aria-expanded` no botão que controla o menu.

### Atributos importantes

- `aria-expanded="false"` → indica que o menu está fechado
- `aria-controls="menu"` → informa qual elemento o botão controla
- `aria-label` → melhora a leitura por leitores de tela

### Por que usar esse padrão

- melhora acessibilidade
- deixa o estado explícito no HTML
- evita depender apenas de classes CSS
- facilita manutenção do JavaScript

### Exemplo

```html
<button
  aria-label="Abrir menu"
  aria-expanded="false"
  aria-controls="menu">
</button>
```