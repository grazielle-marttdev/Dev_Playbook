# Quando usar cada estrutura de pastas

Este guia ajuda a escolher a estrutura de pastas mais adequada para cada tipo de projeto.

---
--

## Tabela de decisão rápida

| Tipo de projeto                  | Estrutura ideal                                           |
|----------------------------------|-----------------------------------------------------------|
| Landing pages / projetos simples | Estrutura simples com `components`                        |
| Projetos médios                  | Estrutura tradicional (`components`, `hooks`, `services`) |
| Projetos grandes                 | Feature-based architecture                                |

---
--

## Estrutura simples

Indicada para:

- landing pages
- projetos de estudo
- pequenos projetos de portfólio

Características:

- poucas pastas
- organização direta
- baixa complexidade

---

## Estrutura tradicional

Indicada para:

- aplicações front-end médias
- projetos com várias páginas
- aplicações que consomem APIs

Características:

- separação por tipo de responsabilidade
- melhor escalabilidade que a estrutura simples

---

## Feature-based architecture

Indicada para:

- aplicações grandes
- sistemas complexos
- projetos com muitas funcionalidades

Características:

- organização por funcionalidade
- melhor isolamento de código
- maior escalabilidade