# Nombre del Proyecto

Proyecto con React y Vite para la creación de una vista que muestra datos mediante JS, renderizado de listas y JSX.

## Inicio rápido

Sigue estos pasos para obtener una copia del proyecto en tu máquina local para desarrollo y pruebas, el proyecto ya incluye un componente dentro de la carpeta `views`, puedes utilizar ese componente o crear uno nuevo. El proyecto es tuyo.

### Clona el repositorio

```bash
git clone git@github.com:jmontes50/challenge_react_1.git

cd challenge_react_1
```

### Instala las dependencias

Recuerda que es necesario instalar las dependencias para que se descarguen en la carpeta node_modules y que el proyecto pueda funcionar correctamente

```bash
npm install
```

### Inicia el servidor de desarrollo

```bash
npm run dev
```

## Uso de estado y efectos

Para lograr la funcionalidad esperada en la aplicación, asegúrate de utilizar los hooks useState y useEffect proporcionados por React. Estos hooks te permitirán gestionar el estado y realizar efectos secundarios cuando sea necesario

```jsx
import React, { useState, useEffect } from 'react';

function MiComponente() {
  const [datos, setDatos] = useState([]);

  useEffect(() => {
    // Lógica para obtener datos de la API 
    // ...

    // Actualiza el estado cuando sea necesario
    setDatos(nuevosDatos);
  }, []); // El segundo argumento vacío significa que se ejecuta solo una vez al montar el componente

  return (
    <div>
      {/* Renderiza la lista utilizando los datos, esto es solo un ejemplo */}
      {datos.map((item) => (
        <div key={item.id}>{item.nombre}</div>
      ))}
    </div>
  );
}

export default MiComponente;

```

## Estilo y Diseño

Se recomienda seguir [principios de diseño](https://www.visily.ai/blog/ui-design-best-practices/) y a utilizar Bootstrap o CSS para mejorar la apariencia visual de la aplicación.

## Datos y API

Se recommienda el uso de [MockAPI](https://mockapi.io/) o una API externa como [reqres.in](https://reqres.in/) para obtener y mostrar datos en las listas renderizadas. Asegúrate de documentar cómo configurar y utilizar estos datos.
