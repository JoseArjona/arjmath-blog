---
title: "Guía Rápida de Markdown"
description: "Guía de la sintaxis markdown"
autor: "Jose Arjona"
pubDate: "02 Nov 2022"
heroImage: "https://pic1.zhimg.com/v2-c93ae95786e7e4f0240ea31de4020083_r.jpg?source=172ae18b"
heroImageAlt: "Markdown logo"
---

## Cabeceras

Usa las almohadillas (#) para crear los encabezados el número de almohadillas es el nivel del encabezado así hasta el 6

#### Sintaxis

```md
# Cabecera nivel 1

## Cabecera nivel 2

### Cabecera nivel 3

#### Cabecera nivel 4

##### Cabecera nivel 5

###### Cabecera nivel 6
```

## Estilos en Texto

Al igual como los encabezados entre más \* agregues cambiara él efecto. Los asteriscos van sin espacio.

| **Sintaxis**  | **Resultado**                    |
| ------------- | -------------------------------- |
| `*Cursiva*`   | _texto en cursiva_               |
| `**negrita**` | **texto en negrita**             |
| `***ambos***` | **_texto en cursiva y negrita_** |
| `~~tachado~~` | ~~tachado~~                      |

## Tablas

#### Sintaxis

```markdown
| Sintaxis| Descripción| Resultado |
| :--- | :----: | ---: | se usa para la alineación
| Header | Title | Here's this |
| Paragraph | Text | And more |
```

> o Usa el generador de tabla : https://www.tablesgenerator.com/markdown_tables

#### Resultado

| Sintaxis  | Descripción |   Resultado |
| :-------- | :---------: | ----------: |
| Header    |    Title    | Here's this |
| Paragraph |    Text     |    And more |

<br>

## Listas y Bloques

<br>

### Bloques de citado

#### Sintaxis

para poner bloques de citado se usa > antes de empezar el texto

```md
> este sería un Resultado
> de como debes escribirlo
```

#### Resultado

> este sería un Resultado
> de como debes escribirlo

### Bloques de código

para poner bloques de código se usa las tres comillas invertidas simples ``` antes y después además, se puede especificar el código usando las tres comillas
y seguido el lenguaje por Resultado json después cierras las comillas invertidas y el código

#### Sintaxis

````md
```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
````

#### Resultado

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### Listas

Para poner listas ordenas simplemente por un numero antes `1.` lista y así.
Para listas no ordenadas solo pon un `-` lista.
Para listas dentro de listas solo usa los espacios.
Y para empezar una lista con numero sin que se ordenen pon \ y el numero

#### Sintaxis

```md
- Lista
- no
- ordenada

1.  Lista
2.  xd
3.  ordenada

- primera item
- segundo item
- tercera item
  - Interna
  - Interna
- cuarto item
```

#### Resultado

- Lista
- no
- ordenada

1.  Lista
2.  xd
3.  ordenada

- primera item
- segundo item
- tercera item
  - Interna
  - Interna
- cuarto item

### Imágenes

Para poner imágenes en markdown tenemos que usar la siguiente estructura
`![Aquí colocamos el alt de la imagen]`+`(Aquí colocamos la ubicación de la imagen)`

#### Sintaxis

```md
![Imagen de una edificación de la Ciudad de Mexico](https://images.pexels.com/photos/604661/pexels-photo-604661.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1 "Imagen de una edificación de la Ciudad de Mexico")
```

#### Resultado

![Imagen de una edificación de la Ciudad de Mexico](https://images.pexels.com/photos/604661/pexels-photo-604661.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1)

### Url

Por ultimo para poner una url en un texto. Similar a como ponemos la imagen solo que ahora invertimos los símbolos colocando `[aquí el texto]`+`(Aquí la url)`

#### Sintaxis

```md
[Mardown Sintaxis completa](https://www.markdownguide.org/basic-syntax/)
```

#### Resultado

[Mardown Sintaxis completa](https://www.markdownguide.org/basic-syntax/)
