# Padrão de Commits

Este documento define o padrão de mensagens de commit utilizado nos meus projetos.

---
--

## Tabela Rápida

| Tipo | Quando usar | Exemplo |
|-----|-----|-----|
| feat | Nova funcionalidade | feat: adiciona menu hambúrguer |
| fix | Correção de bug | fix: corrige erro no botão do menu |
| refactor | Reorganização do código sem alterar comportamento | refactor: reorganiza script do menu |
| style | Alterações visuais ou de formatação | style: ajusta indentação do CSS |
| docs | Alterações na documentação | docs: adiciona guia de commits |
| chore | Tarefas de manutenção | chore: reorganiza estrutura do projeto |
| test | Adição ou modificação de testes automatizados | test: adiciona testes do formulário |

---
--

## Estrutura da Mensagem

Os commits seguem a seguinte estrutura:

```
tipo: descrição curta do que foi feito
```

Exemplo:

```
feat: adiciona menu hambúrguer responsivo

fix: corrige erro na navegação mobile

refactor: melhora organização do código do header
```

--- 

## Tipos de Commit

### ```feat```
Usado quando uma **nova funcionalidade** é adicionada.

Exemplo:
```
feat: adiciona menu hambúrguer para telas mobile
```
---

### ```fix```
Usado para **correção de bugs ou problemas**.

Exemplo:
```
fix: corrige comportamento do botão de menu em telas pequenas
```
---

### ```refactor```
Usado quando o código é **reorganizado ou melhorado sem alterar comportamento**.

Exemplo:
```
refactor: reorganiza funções do menu em módulo separado
```
---

### ```style```
Mudanças que afetam **apenas estilo ou formatação do código**.

Exemplo:
```
style: ajusta indentação do CSS
```
---

### docs
Usado quando **apenas documentação é alterada**.

Exemplo:
```
docs: adiciona explicação sobre acessibilidade do menu
```
---

### ```chore```
Tarefas de manutenção do projeto.

Exemplo:
```
chore: atualiza estrutura de pastas
```

---

### ```test```
Usado quando são **adicionados, modificados ou corrigidos testes automatizados** do projeto.

Esse tipo de commit indica mudanças relacionadas apenas à verificação do funcionamento do código, sem alterar a lógica principal da aplicação.

Exemplo:
```
test: adiciona testes para validação do formulário

test: corrige teste que falhava no menu mobile
```

Boas práticas:
- Cada funcionalidade importante deve ter pelo menos um teste associado
- Testes devem ser claros e fáceis de entender
- Testes devem validar comportamento, não implementação interna

---

## Filosofia

Cada commit deve representar uma mudança clara e específica.

Boas práticas:
- Commits pequenos
- Uma responsabilidade por commit
- Mensagens claras e objetivas
- Explicar *o que foi feito*, não apenas *o arquivo alterado*