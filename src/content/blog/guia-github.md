---
title: "Iniciando en GitHub: Una Guía Rápida"
autor: "Jose Arjona"
description: "Guía Básica y Comandos Básicos Github"
pubDate: "05 Jan 2024"
heroImage: "https://github.blog/wp-content/uploads/2022/01/space-banner.png?resize=1200%2C627"
heroImageAlt: "GitHub logo"
---

GitHub se ha convertido en una herramienta esencial para desarrolladores, permitiendo la colaboración eficiente y el seguimiento de cambios en proyectos. En esta guía rápida, aprenderás los fundamentos para subir, clonar y actualizar proyectos en GitHub, junto con comandos útiles y extensiones recomendadas para Visual Studio Code.

## Subir un proyecto a GitHub

Para comenzar, seleccionamos la carpeta que contiene nuestro proyecto y abrimos una terminal desde allí (clic derecho y seleccionamos "Abrir en terminal").

> Nota: Es crucial asegurarse de estar en la dirección correcta de tu proyecto antes de continuar.

En la terminal, inicializamos el repositorio con el siguiente comando:

```bash
  git init
```

Posteriormente, agregamos todos los archivos al repositorio utilizando:

```bash
 git add .
```

Donde el punto indica que se agregarán todos los archivos. Luego, realizamos el commit con un mensaje descriptivo para identificar el cambio.
El commit significa una confirmación de los cambios.

```bash
 git commit -m "first commit"
```

A continuación, cambiamos la rama del proyecto a "main" (siguiendo la recomendación de GitHub):

```bash
 git branch -M main
```

Por ultimo, asociamos nuestro repositorio local con el repositorio remoto en GitHub mediante:

```bash
 git remote add origin + <URL_del_Repositorio>
```

> Nota: la url va sin `<` `>`. Unicamente se uso para fines descriptivos

Y subimos los archivos al repositorio remoto:

```bash
 git push -u origin main
```

## Clonar un proyecto de GitHub

Para clonar un proyecto desde GitHub, seleccionamos la carpeta donde deseamos clonar el proyecto, abrimos una terminal y ejecutamos:

```bash
git clone <URL_del_Repositorio>
```

### Clonar de una rama en especifico

Si deseamos clonar una rama específica, utilizamos el siguiente comando:

```bash
git clone -b <nombre_de_rama> <URL_del_Repositorio>

```

Donde `<nombre_de_rama>` es el nombre de la rama que queremos clonar.

## Descargar cambios de un proyecto

Cuando otros colaboradores han realizado cambios en el repositorio remoto y deseas incorporar esas actualizaciones a tu versión local, utiliza el siguiente comando:

```bash
git pull
```

Este comando descargará los cambios más recientes del repositorio remoto y los fusionará automáticamente con tu rama local actual. Asegúrate de estar en la rama correcta antes de ejecutar este comando.

## Subir Cambios a GitHub

Cuando hayas realizado modificaciones en tu proyecto y desees subirlas a GitHub, puedes hacer lo siguiente:

#### 1 verifica el estado de tus cambios

```bash
git status
```

Este comando te mostrará los archivos modificados y confirmará que estás en la rama correcta.

#### 2 Agrega los cambios

```bash
git add .
```

El punto indica que se agregarán todos los archivos modificados.

#### 3 Realiza un commit

```bash
git commit -m "Mensaje descriptivo de tus cambios"
```

Proporciona un mensaje descriptivo que resuma los cambios que realizaste. (Trata de ser preciso en tus cambios)

#### Sube los cambios al repositorio remoto:

```bash
git push origin main

```

Este comando subirá tus cambios a la rama principal del repositorio remoto en GitHub. Asegúrate de cambiar "main" si estás trabajando en una rama diferente.

## Comandos utiles

```bash
git status # Muestra el estado del repositorio
git log # Muestra el historial de cambios
git log --oneline # Muestra el historial de cambios en una sola linea
git log --oneline --graph # Muestra el historial de cambios en una sola linea con un grafico
git checkout -b rama # Crea una rama y se cambia a ella
git branch # Muestra las ramas
```

## Extensiones recomendas en VSCODE para github

Estas extensiones en Visual Studio Code nos ayudaran a trabajar con github de una manera mas facil.

- [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
- [GitHub Pull Requests and Issues](https://marketplace.visualstudio.com/items?itemName=GitHub.vscode-pull-request-github)
