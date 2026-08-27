# Hoja de Vida Profesional en HTML5 Nativo

## Información del Estudiante
* **Nombre Completo:** Joaquin Francisco Villalpando Apaza
* **Carrera:** Ingeniería de Sistemas
* **Semestre:** Cuarto Semestre
* **Asignatura:** Tecnologías Web I (SIS-214)
* **Docente:** Ing. MSc. Miguel Angel Pacheco Arteaga
* **Institución:** Universidad Católica Boliviana "San Pablo" (UCB)
* **Fecha de Entrega:** 26 de agosto de 2026

---

## Descripción del Proyecto
Este proyecto consiste en el diseño y desarrollo de una **Hoja de Vida Profesional y Técnica** estructurada bajo estándares rigurosos de **HTML5 Nativo**, aplicando la filosofía de desarrollo sin dependencias (**"Zero Frameworks"**).

El diseño se enfoca en la semántica estructural limpia, accesibilidad nativa de cara al usuario (A11y), visualización cuantitativa de datos, componentes interactivos sin JavaScript y optimización de recursos multimedia para navegadores modernos.

---

## Arquitectura de Directorios (Estructura del Proyecto)
El proyecto se organiza estrictamente bajo la estructura de archivos y rutas de recursos real y funcional del entorno de desarrollo local:

```text

hoja-vida/

├── index.html
├── README.md
└── assets/
    ├── audio/
    │   ├── presentacion_personal.mp3
    │   └── presentacion_personal.ogg
    ├── documents/
    │   └── hoja-de-vida-completa.pdf
    ├── images/
    │   ├── foto-perfil.JPG
    │   └── video-poster.png
    └── video/
        ├── video-hoja-vida.mp4
        └── video-hoja-vida.webm
```

---

## Requisitos Técnicos e Implementación Semántica

### 1. Semántica Estructural (Arquitectura de Bloques)
Se implementaron de forma exclusiva las etiquetas semánticas del estándar moderno para evitar la "sopa de divs", organizando el documento de la siguiente manera:

* **`<header>`:** Contiene la presentación principal, fotografía profesional bajo elemento adaptativo, datos de contacto y metadatos accesibles.
* **`<nav>`:** Menú de navegación principal con hipervínculos internos ancla para un desplazamiento rápido entre secciones.
* **`<main id="contenido-principal">`:** Escenario central único que encapsula el contenido principal de la hoja de vida.
* **`<section>`:** Bloques temáticos independientes e identificables con identificadores únicos (`#perfil`, `#estudios`, `#experiencia`, `#habilidades`, `#certificaciones`, `#idiomas`, `#proyectos`, `#multimedia`, `#contacto`).
* **`<article>`:** Encapsula de forma independiente cada proyecto académico destacado.
* **`<aside>`:** Barra lateral de contenido complementario para la disponibilidad actual del estudiante, avisos y descarga de archivos.
* **`<footer>`:** Cierre del documento con metadatos de autoría y fecha de última actualización.

### 2. Semántica Inline de Precisión (Semántica de Texto)
Para enriquecer semánticamente el flujo textual de la información se utilizaron etiquetas específicas:

* **`<abbr>`:** Explicación detallada de siglas institucionales (`UCB`, `Ing. de Sistemas`).
* **`<time>`:** Definición formal de fechas y periodos de tiempo procesables para máquinas utilizando el atributo `datetime`.
* **`<mark>`:** Resaltado visual de hitos y logros académicos destacados.
* **`<dfn>`:** Declaración precisa de términos y objetivos profesionales dentro de la introducción.
* **`<dl>, <dt>, <dd>`:** Listas de definiciones estructuradas para organizar y clasificar fortalezas profesionales de forma accesible.

### 3. Componentes Interactivos Nativos (Zero JavaScript)

* **Acordeones Nativo Plegables (`<details>` y `<summary>`):** Utilizados para organizar la formación académica y la experiencia práctica, permitiendo al evaluador contraer y expandir los registros de forma dinámica.
* **Cuadros de Diálogo Nativos (`<dialog open>`):** Aviso interactivo emergente de audiciones en la sección lateral, controlable mediante un formulario nativo con `method="dialog"` para cerrar el aviso.

### 4. Visualización cuantitativa de datos y Tablas Accesibles

* **`<progress>`:** Representación cuantitativa y visual de los niveles de dominio en lenguajes y tecnologías.
* **`<meter>`:** Indicadores visuales nativos con especificación de rangos (`min`, `max`, `low`, `high`, `optimum`) para evaluar competencias lingüísticas y el estado de disponibilidad del estudiante.
* **Tabla de Idiomas Semántica:** Estructura completa bajo estándares de accesibilidad utilizando `<caption>`, `<thead>`, `<tbody>`, y encabezados con `scope="col"` y `scope="row"` para que sea perfectamente interpretada por lectores de pantalla.

### 5. Portafolio Multimedia Adaptativo y Compatible

* **Imagen Responsiva (`<picture>`):** Integración de múltiples fuentes de origen (`<source>`) para la fotografía profesional que se adaptan al hardware del navegador, junto con carga diferida (`loading="lazy"`) para un rendimiento de carga optimizado.
* **Reproductor de Audio Nativo (`<audio>`):** Compatibilidad multiplataforma nativa mediante el uso de fuentes alternativas de códecs de audio en formatos comprimidos estándar (`.mp3` y `.ogg`).
* **Reproductor de Video Nativo (`<video>`):** Elemento multimedia optimizado con imagen de portada (`poster="assets/images/video-poster.png"`) y formatos de códec alternativos (`.mp4` y `.webm`), controlando el ancho nativamente a `width="480"` para su maquetación responsiva.

### 6. Formularios con Validación por Hardware

* **Agrupación Semántica:** Campos de entrada segmentados lógicamente bajo etiquetas `<fieldset>` con sus respectivas descripciones `<legend>`.
* **Controles Avanzados HTML5:** Uso de inputs específicos para teléfonos (`type="tel"`), correos (`type="email"`) y autocompletado semántico nativo mediante `<datalist>`.
* **Validaciones sin JavaScript:** Validación estricta en el cliente gestionada nativamente por el motor del navegador mediante atributos de obligatoriedad (`required`), límites de longitud (`minlength`, `maxlength`) y expresiones regulares (`pattern`) que controlan las restricciones de caracteres para evitar la inyección de datos corruptos.

---

## Instrucciones para Despliegue Local

1. Asegúrese de clonar o descargar este repositorio de forma íntegra manteniendo la jerarquía de directorios descrita en la arquitectura de archivos.
2. Abra la carpeta del proyecto en su editor de código preferido (se recomienda Visual Studio Code).
3. Ejecute un servidor local (por ejemplo, utilizando la extensión **Live Server** en VS Code) o abra directamente el archivo `index.html` en un navegador web moderno compatible con el estándar HTML5 para experimentar todo el flujo multimedia y las validaciones nativas.
