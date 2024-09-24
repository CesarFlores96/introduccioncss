# Clase básica de Css


Es un lenguaje para dar estilos a la web (1996)

## Sintaxis
- Como se puede establecer codigo css
```css
h1 {
    color : red;
}
```

- h1 : Selector
- color : Propiedad
- red : Valor

## CONCEPTOS IMPORTANTES CSS

- 4 Conceptos importantes de CSS

### SELECTORES

- Indica a que elemento o elementos, se aplicara estilos
```css
/* SELECTOR DE ETIQUETA*/
h1 {
    color : red;
}
/* SELECTOR DE DESCEDENCIA*/
nav ul li a {
    color : red;
}
```

### HERENCIA

- Elementos ancestros / padre heredan algunas propiedades a sus descedientes.

- *`La propiedad inherit realiza que se herede de forma forsoza`*

```css
p{
    color: rgb(48, 80, 185);
    font-weight: 600;
}
a{
    color: inherit;
    text-decoration: none;
}
```
### CASCADA

- Los estilos que llegan en ultimo lugar sobreescriben a los anteriores
- *`La especifidad vence a la cascada`*

```css
/* Antiguo Valor*/
h1 {
    color : red;
}
/* Nuevo Valor*/
h1{
    color: cadetblue;
}
```

### ESPECIFICADO

- Es un valor numerico que adquieren los selectores y se aplica cuando hay conflictos


```css
/* Selector de Etiqueta(1)*/
h1 {
    color : red;
}
/* Selector de Clase(10)*/
h1{
    color: cadetblue;
}
/* Selector de ID(100)*/
/* INLINE(1000)*/
/* IMPORT(1000)*/
```