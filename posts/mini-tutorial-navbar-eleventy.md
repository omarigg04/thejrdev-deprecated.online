---
title: Cómo Agregar Dinámicamente Páginas al Navbar con Eleventy
description: Este artículo proporciona un mini tutorial sobre cómo agregar dinámicamente páginas al navbar 
date: 2024-26-07
tags:
  - eleventy
  - tutorial
  - navbar
  - webdevelopment
layout: layouts/post.njk
---

# Mini Tutorial sobre Cómo Agregar Dinámicamente Páginas al Navbar con Eleventy

En este tutorial, aprenderás a agregar dinámicamente páginas a la barra de navegación (navbar) de tu sitio web utilizando la configuración de `eleventyNavigation` en archivos .md o .njk. Eleventy es un generador de sitios estáticos que facilita la creación de sitios web rápidos y eficientes.

## Introducción

Agregar elementos de navegación dinámicamente puede simplificar la gestión de tu sitio web, permitiéndote actualizar el navbar sin modificar múltiples archivos manualmente. Eleventy ofrece una solución sencilla mediante el uso de `eleventyNavigation`.

![Eleventy Navigation](Una ilustración de una configuración de navbar dinámica utilizando Eleventy en un sitio web)

## Paso 1: Configurar el Header en el Archivo .md o .njk

Para agregar una página al navbar, debes incluir la configuración de `eleventyNavigation` en el encabezado de tu archivo .md o .njk. Aquí tienes un ejemplo de cómo hacerlo:

### Ejemplo en un Archivo .md

```markdown
---
title: Short bits
description: Este artículo es sobre bits cortos.
date: 2024-26-07
tags:
  - bits
  - tutorial
layout: layouts/post.njk
eleventyNavigation:
  key: Short bits
  order: 1
---
```

### Ejemplo en un Archivo .njk

```njk
---
title: Short bits
description: Este artículo es sobre bits cortos.
date: 2024-26-07
tags:
  - bits
  - tutorial
layout: layouts/post.njk
eleventyNavigation:
  key: Short bits
  order: 1
---
```

En ambos ejemplos, la configuración de `eleventyNavigation` incluye un `key` que identifica el elemento de navegación y un `order` que determina su posición en el navbar.

## Paso 2: Configurar el Navbar en el Layout Principal

Una vez que has agregado la configuración a tus archivos de contenido, necesitas actualizar el layout principal para generar el navbar dinámicamente. Aquí tienes un ejemplo de cómo hacerlo en un archivo de layout .njk:

```njk
<nav>
  <ul>
    {% for item in collections.eleventyNavigation %}
      <li><a href="{{ item.url }}">{{ item.data.eleventyNavigation.key }}</a></li>
    {% endfor %}
  </ul>
</nav>
```

Este código recorre todos los elementos de `eleventyNavigation` y genera un enlace para cada uno en el navbar.

## Paso 3: Compilar y Verificar

Después de realizar estos cambios, compila tu sitio con Eleventy ejecutando el siguiente comando en tu terminal:

```bash
npx eleventy
```

Verifica que los elementos de navegación aparezcan correctamente en el navbar de tu sitio web.

## Conclusión

Utilizar `eleventyNavigation` para agregar dinámicamente páginas al navbar simplifica la gestión de tu sitio web y asegura que tu navegación esté siempre actualizada. ¡Prueba esta técnica en tu próximo proyecto con Eleventy y disfruta de una gestión de contenidos más eficiente!
