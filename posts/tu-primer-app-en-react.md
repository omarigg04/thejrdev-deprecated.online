---
title: Tu Primer App en React
description: Este artículo proporciona una guía paso a paso sobre cómo crear tu primera aplicación en React, desde la instalación hasta la creación de componentes básicos.
date: 2024-27-07
tags:
  - DIY
  - react
  - tu primer app
  - reactApp
  - web
  - programacion
  - jrdev
  - jr
  - desarrolloweb
  - software
layout: layouts/post.njk
concept: tutorial
---

# Tu Primer App en React

Crear tu primera aplicación en React puede parecer una tarea desalentadora, pero con esta guía paso a paso, estarás en camino de desarrollar aplicaciones web interactivas en poco tiempo. En este tutorial, cubriremos la instalación de React, la creación de un proyecto nuevo, y cómo construir y renderizar componentes básicos.

## ¿Qué es React?

React es una biblioteca de JavaScript desarrollada por Facebook para construir interfaces de usuario. Es especialmente útil para crear aplicaciones de una sola página (SPA) donde necesitas una experiencia de usuario rápida y dinámica.

## Instalación de Node.js y npm

Antes de empezar a trabajar con React, necesitas tener Node.js y npm (Node Package Manager) instalados en tu computadora.

1. **Descargar Node.js**: Visita [nodejs.org](https://nodejs.org) y descarga la versión LTS recomendada.
2. **Verificar la instalación**:
   ```bash
   node -v
   npm -v
   ```

## Crear una nueva aplicación React

React proporciona una herramienta llamada Create React App que simplifica la creación de una nueva aplicación React. Sigue estos pasos para crear tu primer proyecto React:

1. **Instalar Create React App**:
   ```bash
   npx create-react-app mi-primera-react-app
   ```
2. **Navegar al directorio del proyecto**:
   ```bash
   cd mi-primera-react-app
   ```
3. **Iniciar la aplicación**:
   ```bash
   npm start
   ```

Tu nueva aplicación React ahora debería estar ejecutándose en `http://localhost:3000`.

## Estructura del Proyecto

La estructura básica de un proyecto creado con Create React App es la siguiente:

```
mi-primera-react-app/
├── node_modules/
├── public/
├── src/
│   ├── App.css
│   ├── App.js
│   ├── App.test.js
│   ├── index.css
│   ├── index.js
│   └── logo.svg
├── .gitignore
├── package.json
├── README.md
└── yarn.lock
```

## Creación de Componentes Básicos

React se basa en componentes. Vamos a crear un componente simple que muestre un saludo.

1. **Crear un nuevo archivo de componente**: Dentro del directorio `src`, crea un archivo llamado `Saludo.js`.
2. **Definir el componente**:
   ```javascript
   import React from 'react';

   function Saludo() {
     return <h1>¡Hola, mundo!</h1>;
   }

   export default Saludo;
   ```
3. **Usar el componente en App.js**:
   ```javascript
   import React from 'react';
   import Saludo from './Saludo';

   function App() {
     return (
       <div className="App">
         <header className="App-header">
           <Saludo />
         </header>
       </div>
     );
   }

   export default App;
   ```

## Conclusión

¡Felicidades! Has creado tu primera aplicación en React y has aprendido a crear y usar componentes básicos. Desde aquí, puedes explorar más sobre React y sus características avanzadas como el manejo del estado, efectos, y el enrutamiento.

## FAQ

### ¿Qué es Create React App?
Create React App es una herramienta oficial para crear aplicaciones React sin necesidad de configurar un entorno complejo.

### ¿Puedo usar otras herramientas además de Create React App?
Sí, hay otras herramientas y boilerplates como Next.js y Gatsby para aplicaciones más avanzadas.

### ¿Dónde puedo aprender más sobre React?
Puedes encontrar documentación y tutoriales adicionales en la [documentación oficial de React](https://reactjs.org/docs/getting-started.html).

![Crear nueva aplicación React](Una computadora mostrando el terminal con el comando `npx create-react-app mi-primera-react-app` ejecutado y la aplicación en funcionamiento en un navegador.)

---

Espero que este artículo sea útil para que empieces con React. Si tienes alguna pregunta, no dudes en dejar un comentario.
