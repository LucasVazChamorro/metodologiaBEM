# Uso da Metodologia BEM no Projeto

Este projeto utiliza a metodologia BEM (Block Element Modifier) para organizar e estruturar o CSS. BEM é uma convenção de nomenclatura que ajuda a criar componentes reutilizáveis e modulares em front-end.

## O que é BEM?

BEM significa Block Element Modifier:

- **Block**: O componente pai autônomo
- **Element**: Um componente filho que é parte de um Block
- **Modifier**: Uma variação ou estado de um Block ou Element

## Como BEM é Aplicado neste Projeto

### Blocks

No nosso código, temos dois principais Blocks:

1. `.produtos-grid`: Representa a grade de produtos
2. `.produto`: Representa um item de produto individual

### Elements

Elements são indicados por dois underscores (`__`) após o nome do Block:

- `.produto__imagem`: A imagem do produto
- `.produto__nome`: O nome do produto
- `.produto__descricao`: A descrição do produto

### Modifiers

Modifiers são indicados por dois hífens (`--`) após o nome do Block ou Element:

- `.produto--destaque`: Uma variação do produto que está em destaque

## Exemplo de Uso

```css
.produto {
    /* Estilos base para o bloco produto */
}

.produto__imagem {
    width: 100%;
}

.produto__nome {
    font-size: 1.2em;
    margin: 8px 0;
}

.produto--destaque {
    border: 2px solid gold;
    padding: 8px;
    background-color: #ffff42;
}
```

## Benefícios do BEM

1. **Clareza**: A estrutura do HTML pode ser entendida apenas olhando para as classes CSS.
2. **Modularidade**: Os componentes podem ser facilmente reutilizados em diferentes partes do projeto.
3. **Manutenibilidade**: É fácil entender a relação entre diferentes partes do código.

Ao seguir esta metodologia, mantemos nosso CSS organizado, escalável e fácil de manter.