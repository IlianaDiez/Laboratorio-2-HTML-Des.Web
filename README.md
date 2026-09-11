Laboratorio #2 - Desarrollo Web

Instructor: Irina Fong
Grupo: 1S3122

## Tecnología Utilizada
* HTML5: Utilizado para crear la estructura semántica de las páginas, tablas y formularios.
* CSS3: Utilizado para aplicar estilos, selectores de clase e ID, y mejorar la presentación visual de cada ejercicio.
* PHP: Utilizado en el ejercicio de validación de formulario (saneamiento y validación de datos).
* Git: Utilizado para el control de versiones del proyecto.
* GitHub: Utilizado para almacenar el repositorio del laboratorio.
* WampServer: Utilizado como servidor local para ejecutar y probar el archivo PHP de validación.

## Información relevante del laboratorio
Durante el Laboratorio #2 - Desarrollo Web se trabajaron los temas de configuración y metadatos del documento, elementos semánticos de HTML5, tablas HTML, hipervínculos y selectores CSS, aplicando buenas prácticas de organización, comentarios explicativos y hojas de estilo externas e internas.

### 1. Tabla #1 - Informe de Gastos de Viaje (`Tablas1.html`)
- Se construyó una tabla HTML con la etiqueta `<table>`, utilizando `<th>` para las cabeceras y `<td>` para las celdas de datos.
- Se implementaron los atributos `id`, `axis` y `headers` para relacionar cada fila de datos con su cabecera correspondiente (Buenos Aires y Córdoba), mejorando la accesibilidad de la tabla.
- Se agregaron metadatos de configuración: `charset="UTF-8"`, `viewport`, `description`, `keywords`, `author` y `robots`.
- Se agregó un ícono de acceso directo (favicon) mediante `<link rel="shortcut icon" href="imagen/icono.png">`, guardado dentro de la carpeta `imagen/`.
- Se aplicaron estilos CSS internos para dar bordes y líneas a la tabla (`border-collapse`, `border`, `padding`).

### 2. Tabla #2 - Reporte de Ventas (`tablas2.html` + `Estilos/estilosTabla.css`)
- Se construyó una segunda tabla utilizando una hoja de estilos CSS externa, vinculada mediante `<link rel="stylesheet">`.
- Se definieron selectores de clase reutilizables: `.tabla`, `.tabla th`, `.tabla .modo1`, `.tabla .modo1 td`, `.tabla .modo2` y `.tabla .modo2 td`, para dar un formato distinto a filas alternas.
- Se practicó la diferencia de comportamiento por defecto entre `<th>` (negrita y centrado) y `<td>`.

### 3. Párrafos y Selectores Descendientes (`parrafos.html` + `Estilos/estilosParrafos.css`)
- Se trabajó con las etiquetas `<q>` (cita en línea) y `<strong>` (importancia fuerte).
- Se aplicó el selector descendiente `p strong`, el cual estiliza cualquier elemento `<strong>` contenido dentro de un `<p>`, sin importar el nivel de anidación.

### 4. Navegación Web con Clases e ID (`Ejemplo2.html`)
- Se creó una sección (`<section>`) estilizada con la clase reutilizable `.card-seccion`.
- Se implementó un hipervínculo externo seguro utilizando los atributos `target="_blank"` y `rel="noopener"`, evitando riesgos de seguridad relacionados con `window.opener`.
- Se utilizó un `<footer>` con un ID único (`#footer-recurso`) para dar estilo a un elemento específico dentro del documento.

### 5. Estructura Semántica de HTML5 (`Ejemplo5.html`)
- Se construyó una página utilizando las etiquetas semánticas `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>` y `<footer>`.
- Se aplicaron estilos CSS diferenciados por color de fondo a cada bloque, para visualizar claramente la organización estructural del documento.

### 6. Validación de Formulario (`Validacion.php`)
- Se desarrolló un formulario para ingresar nombre y edad, con validación de datos en PHP.
- Se validó el nombre utilizando una expresión regular (`preg_match` con `\p{L}\s`) para permitir únicamente letras y espacios, rechazando números y caracteres especiales.
- Se utilizó `mb_convert_case()` para convertir automáticamente la primera letra de cada palabra del nombre en mayúscula.
- Para la edad se utilizó `filter_var(..., FILTER_VALIDATE_INT)`, con un rango válido de 0 a 120 años.
- Se agregó una lista de errores acumulados, `htmlspecialchars()` en la salida como buena práctica de seguridad, y comentarios explicativos.

## Cumplimiento de lo solicitado
- Se realizaron los ejemplos indicados en la guía del laboratorio: tabla #1, tabla #2, párrafos con selectores descendientes, navegación con clases e ID, y estructura semántica de HTML5.
- Los ejercicios fueron ejecutados y probados mediante un servidor local con WampServer.
- Se organizó el proyecto en un repositorio de GitHub para realizar la entrega correspondiente en Moodle.
- Se incluyeron comentarios en los archivos HTML, CSS y PHP para explicar las partes principales del código.
- Como valor agregado, se incorporó un ícono de acceso directo (favicon), validación de datos con expresiones regulares y saneamiento de entradas en el formulario.

## Conclusión
El laboratorio permitió reforzar los conocimientos de HTML5 y CSS3 mediante la creación de tablas de datos, el uso de elementos semánticos, la implementación de hipervínculos seguros y la aplicación de selectores CSS (de clase, de ID y descendientes). Además, se practicó la organización de un proyecto web en carpetas separadas para estilos e imágenes, y se aplicaron buenas prácticas de seguridad y validación en el formulario desarrollado con PHP.

## Estructura del repositorio
```
Lab2/
├── Estilos/
│   ├── estilosTabla.css
│   └── estilosParrafos.css
├── imagen/
│   └── icono.png
├── Tablas1.html
├── tablas2.html
├── parrafos.html
├── Ejemplo2.html
├── Ejemplo5.html
├── Validacion.php
└── README.md
```
