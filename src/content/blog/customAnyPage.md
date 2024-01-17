---
title: "Personaliza cualquier página web con las DevTools"
description: "Cómo personalizar cualquier página web con los Overrides de DevTools."
autor: "Jose Arjona"
pubDate: "13 Aug 2023"
heroImage: "https://images.pexels.com/photos/1779487/pexels-photo-1779487.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
heroImageAlt: "OptimizarWebImg"
---

¿Te gustaría cambiar el aspecto de cualquier página web a tu gusto? ¿Quieres probar diferentes diseños, colores, fuentes o imágenes sin tener que modificar el código fuente? Pues con los Overrides de DevTools puedes hacerlo fácilmente. Los Overrides de DevTools son una función de las herramientas de desarrollo de Chrome (o cualquier navegador con Chromium) que te permiten modificar el HTML, CSS y JavaScript de una página web y ver los cambios en tiempo real y mantenerlos. En este post te voy a enseñar cómo usar los Overrides de DevTools para personalizar cualquier página web.

## Caso de uso

¿Alguna vez has visitado una página web cuyo texto era demasiado pequeño o grande? ¿O tal vez el color del texto no era muy contrastante con el fondo? Si este es el caso, puedes usar los Overrides de DevTools para personalizar el aspecto de la página y hacerla más fácil de leer. El límite es tu imaginación, paciencia y tus habilidades de CSS.

## Paso a paso

1. Primero,abre la página web que quieres personalizar en Chrome.
2. Abre las herramientas de desarrollo de Chrome haciendo clic en el botón "Más herramientas" y luego seleccionando "Herramientas para desarrolladores" o presiona `f12`.
3. En la ventana de herramientas de desarrollo, haz clic en la pestaña "Fuentes" (Sources).
4. Después aparecerán subpestañas. Selecciona la que dice "Invalidaciones" (Overrides). _Si la opición no te sale presiona el simbolo '>>' en la sub pestaña._ ![Imagen Pestañas DevTools](../../assetsBlog/dvtools.png)
5. La primera vez te pedirá que subas una carpeta, así que crea una carpeta en tu dispositivo y súbela.
6. Luego, activa la [x] casilla de Habilitar reemplazos locales.
7. Ahora puedes ir a la subpestaña de "Página" y modificar lo que deseas o ir a la pestaña "Elementos".
8. Las cosas que modifiques tendrán un círculo morado y se guardarán en la carpeta de Overrides o como la hayas nombrado.
9. Los cambios se aplicarán a la página web en tiempo real.

> 🚨 Importante, asegúrate de guardar los cambios antes de recargar.

### Eliminar Overrides

Puede que modifiques demasiado y requieras reiniciar a los valores predeterminados. Para ello ve a la subpestaña de "Invalidaciones" (overrides) y dentro de la carpeta que subiste la primera vez, elimina la carpeta con el nombre del sitio. Por lo general será `web.nombredelsitio.com`.

### Tip

Si al recargar o salirte de la página no ves tus estilos, abre las devtools otra vez, estos estilos deberían cargar.

## Conlusión

En conclusión, los Overrides de DevTools son una herramienta muy útil para personalizar el aspecto de las páginas web. Con esta herramienta, puedes hacer que las páginas web sean más fáciles de leer y más agradables a la vista. También puedes usar los Overrides de DevTools para probar diferentes diseños, colores, fuentes o imágenes sin tener que modificar el código fuente. Esto te permite experimentar con diferentes opciones y ver cómo se vería la página web con diferentes configuraciones.
