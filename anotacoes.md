# Tags semânticas

```html
<header> </header>

<nav> </nav>

<main> </main>

<section> </section>

<article> </article>

<aside> </aside>

<footer> </footer>
```

- `header`: Cria um grupo de suporte introdutório, navegacional, pode ser utilizado para campo de busca, logo do site, links de navegação, dentre outros.

- `nav`: Muito utilizada para criar menus, representa uma seção de link de navegação. Podem existir várias

- `main`: Conteúdo principal da página. Pode existir apenas uma por página.

- `section`: Representa uma sessão genérica, podem existir várias por página.

- `article`: Um exemplo é, em um blog, essa tag representará um trecho.

- `aside`: Pode ser utilizado para barras laterais, menu lateral. Pode ser usado tanto o `<nav>` quando o `<aside>`

- `footer`: Representa o rodapé da página.

A tag `div` serve para arranjar o layout, montando containers.

---

# CSS

### Unidades de medida

- `vh`: pega a altura máxima e dividir em 100 partes iguais.

- `rem`: unidade de medida **relativa**. Em diferentes dispositivos, apresenta um layout fluido.

### Seletores

| Seletor | sintaxe |
|:----:|:----:|
| classe | .nomeclasse |
| ID | #idDoElemento |
| tag | body |

Para cliar um flexbox, criamos uma div e estilizamos utilizando a seguinte sintaxe:

```css
.header-content {
    display: flex;
    justify-content: space-between;
}
```

Por padrão o `display: flex` a direção padrão é `inline`.

A sintaxe para criar uma variável em CSS é:

```css
:root {
    --background-gray: #ffffff;
}
```

Para "invocar" esta variável, usamos a função `var()`:

```css
* {
    background-color: var(--background-gray);
}
```

Link de referência: https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties


A tag `<span></span>` tem uso genérico.

A sintaxe abaixo construiu, ao invés do texto "menu" e "avatar", os ícones respectivamente:

```html
    <head>
        <link href="https://fonts.googleapis.com/css2?family=Material+Icons+Outlined"
            rel="stylesheet">
    </head>
                <div>
                    <span class="material-icons-outlined">menu</span>
                </div>

                <!-- Avatar -->
                <div><span class="material-icons-outlined">account_circle</span></div>
            </div>
```

Quando colocamos o código abaixo:  

```css 
.avatar {
    font-size: 2rem !important;
}
```
estamos dizendo que o tamanho de fonte de `2rem` é mais importante do que o tamanho que ele herdou da classe (no caso o material-icons-outlined).

Com o `display: grid;` conseguimos utilizar um grid container.

A responsividade é pela sintaxe abaixo:

```css
@media screen and (max-width: 375px) {
}
```

Para conseguir navegar pelo teclado usando a tecla `tab` precisa da sintaxe: 

```html
<span tabindex="1" (...)></span>
```

Para ter texto alternativo, usar a sintaxe:

```html
<a aria-label="descrição básica" class="nav-link">
```