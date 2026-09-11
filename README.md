# Laboratorio #2 - Desarrollo Web

**Instructor:** Irina Fong
**Grupo:** 1S3122

---

## 🛠️ Tecnología Utilizada
* HTML5: Utilizado para crear la estructura semántica de las páginas, tablas y formularios.
* CSS3: Utilizado para aplicar estilos, selectores de clase e ID, y mejorar la presentación visual de cada ejercicio.
* Git: Utilizado para el control de versiones del proyecto.
* GitHub: Utilizado para almacenar el repositorio del laboratorio.
* WampServer: Utilizado como servidor local para ejecutar y probar los archivos del laboratorio.

---

## 📋 Información relevante del laboratorio
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

### 6. Validación Nativa de Formularios con HTML5 y CSS (`ValidacionesHTML5.html`)
- Se implementó un campo de formulario (`type="email"`) con el atributo `required` para validación nativa del navegador, sin necesidad de JavaScript ni un lenguaje de servidor.
- Se utilizaron las pseudo-clases de CSS `:required:valid` y `:required:invalid` para cambiar dinámicamente el color del borde del campo (verde si es válido, rojo si no lo es), según el estado de validación del navegador.

---

## ✅ Cumplimiento de lo solicitado
- Se realizaron los ejemplos indicados en la guía del laboratorio: tabla #1, tabla #2, párrafos con selectores descendientes, navegación con clases e ID, estructura semántica de HTML5 y validación nativa de formularios con CSS.
- Los ejercicios fueron ejecutados y probados en el navegador web, algunos directamente desde el disco y otros mediante un servidor local con WampServer.
- Se organizó el proyecto en un repositorio de GitHub para realizar la entrega correspondiente en Moodle.
- Se incluyeron comentarios en los archivos HTML y CSS para explicar las partes principales del código.
- Como valor agregado, se incorporó un ícono de acceso directo (favicon) dentro de una carpeta dedicada de imágenes.

---

## 🎯 Conclusión
El laboratorio permitió reforzar los conocimientos de HTML5 y CSS3 mediante la creación de tablas de datos, el uso de elementos semánticos, la implementación de hipervínculos seguros, la aplicación de selectores CSS (de clase, de ID y descendientes) y la validación nativa de formularios mediante pseudo-clases de CSS. Además, se practicó la organización de un proyecto web en carpetas separadas para estilos e imágenes, aplicando buenas prácticas de comentarios y metadatos de configuración.

---

## 📁 Estructura del repositorio
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
├── ValidacionesHTML5.html
└── README.md
```
