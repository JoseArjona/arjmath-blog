---
title: "3 Trucos con CSS para mejorar tu web"
description: "Tres trucos usando css para mejorar cualquier pagina web."
autor: "Jose Arjona"
pubDate: "18 Jan 2024"
heroImage: "https://onedrive.live.com/embed?resid=8330862F54B93ABA%21484&authkey=%21AJyrxDsqXvQQ7cY&width=1680&height=945"
heroImageAlt: "Tres trucos css"
---

El mundo del desarrollo web está lleno de posibilidades, y hoy quiero compartir tres trucos increíbles que puedes lograr ¡usando solo CSS! Estos le darán un impulso a la apariencia y funcionalidad de tu sitio web.

## Botón para subir al top de la página

Este truco es muy útil cuando tienes una página web con mucho contenido y quieres que los usuarios puedan volver fácilmente al principio de la página. (Se que existe una forma con JS, pero con CSS mejoraras el rendimiento de tu web)

Primero podemos usar el desplazamiento suave, añadiendo el `scroll-behavior: smooth;` a nuestro body. Esto con el fin de no hacer una animación tan brusca al subir en la pagina.

```css
html {
  scroll-behavior: smooth;
}
```

El truco radica en que juguemos con el margen top del `anchor` para hacer que nuestro botón aparezca en la parte más baja de nuestra pagina. Y proporcionando algunos estilos para su posicionamiento. Y usando `#top` nos dirigimos a la parte superior de la pagina.

```html
<a id="back-top" href="#top"> Arriba </a>
```

```css
#back-top {
  margin-top: 115vh;
  position: sticky;
  bottom: 32px;
  left: 90vw;
  padding: 10px;
}

#back-top {
  background: white;
  border-radius: 1000px;
  box-shadow: 0 0 10px #00000035;
  background: rgb(86, 15, 136);
  color: #fff;
  text-decoration: none;
}
```

Si deseamos que nuestro botón aparezca después o antes de cierto contenido jugamos con el `margin-top`

## Validación Visual de formularios con CSS

La validación de formularios es crucial, y ahora puedes hacerla visual sin usar JavaScript adicional. Utilizando el atributo :valid en combinación con HTML5, puedes cambiar el estilo de los elementos de tu formulario en función de su validez.

```html
<form>
  <label for="email"
    >Correo Electrónico:
    <input type="email" id="email" name="email" required />
  </label>
</form>
```

```css
label:has(:focus:invalid) {
  color: rgb(255, 130, 107);
}
label:has(:focus:valid) {
  color: rgb(53, 113, 53);
}
```

Este código hará que el color de texto se ponga rojizo si no tiene ningún valor.Podemos usar este truco para validar cualquier tipo de elemento de formulario

## Modificación del scroll de una página

Este truco nos permite modificar el scroll de una página de forma personalizada con CSS. Es muy conocido, pero realmente le agrega un toque especial a nuestra pagina.

```css
/* Para navegadores WebKit como Chrome y Safari */
::-webkit-scrollbar {
  /* Ancho de la barra de desplazamiento */
  width: 5px;
}

::-webkit-scrollbar-thumb {
  /* Color de la barra de desplazamiento */
  background-color: #e4b92b;
  /* Bordes redondeados del botón de desplazamiento */
  border-radius: 6px;
}

::-webkit-scrollbar-track {
  /* Color de fondo de la barra de desplazamiento */
  background-color: #191720;
}
```

Incluso podemos agregar los pseudoelementos de :hover

```css
/* Color del botón de desplazamiento al pasar el ratón */
::-webkit-scrollbar-thumb:hover {
  background-color: #555;
}
/* Color de fondo de la barra de desplazamiento al pasar el ratón */
::-webkit-scrollbar-track:hover {
  background-color: #d4d4d4;
}
```

Estos trucos de CSS no solo harán que tu sitio web se vea más profesional, sino que también mejorarán la experiencia del usuario. ¡Inténtalos y lleva tu web al siguiente nivel!.
