# Portafolio personal | Luis Alberto Chávez Toussaint

Sitio web personal y responsivo creado para presentar mi perfil como desarrollador web junior, las tecnologías que utilizo, algunos de mis proyectos y mis medios de contacto.

Este proyecto fue desarrollado durante el sprint 4 del programa de Desarrollo Web de TripleTen y también funciona como una muestra práctica de mis conocimientos de HTML, CSS, diseño responsivo, metodología BEM y publicación con GitHub Pages.

## Demo

[Ver el portafolio publicado](https://allenprkr.github.io/web_project_portfolio_es/)

## ¿Por qué se creó este proyecto?

Un currículum tradicional permite resumir la experiencia de una persona, pero no siempre muestra cómo aplica sus conocimientos. Por esta razón, el portafolio se creó como una carta de presentación digital en la que visitantes, reclutadores y posibles colaboradores pueden:

- conocer mi perfil profesional;
- identificar rápidamente mis habilidades técnicas;
- consultar ejemplos de proyectos terminados;
- acceder al código fuente y a las demostraciones publicadas;
- descargar mi currículum;
- comunicarse conmigo mediante correo electrónico o redes sociales.

Además de cubrir esa necesidad, el proyecto me permitió practicar la transformación de un diseño visual en una interfaz web adaptable a distintos tamaños de pantalla.

## Objetivo

El objetivo principal es reunir mi información profesional en un sitio claro, accesible y fácil de consultar. La interfaz busca comunicar quién soy, qué herramientas manejo y qué he construido, sin requerir registros, formularios ni pasos adicionales por parte del visitante.

## Funcionalidades

- Presentación del perfil profesional con fotografía y descripción breve.
- Descarga directa del currículum en formato PDF.
- Enlace al perfil de GitHub y navegación interna hacia la sección de contacto.
- Listado visual de habilidades y herramientas.
- Tarjetas de proyectos con descripción, tecnologías, logros, demo y repositorio.
- Enlaces de contacto por correo electrónico, LinkedIn, Facebook, Instagram y X.
- Diseño adaptable para escritorio, tableta y teléfono móvil.
- Efectos visuales de interacción mediante estados `:hover`.
- Desplazamiento suave hacia las secciones internas.

## ¿Cómo funciona?

El portafolio es un sitio estático: el navegador carga `index.html`, que contiene la estructura y el contenido principal, y después importa `styles/index.css`. Este archivo centraliza la carga de las hojas de estilo de cada sección.

El contenido se organiza en cuatro bloques:

1. **Perfil:** muestra el nombre, la especialidad, una introducción, la fotografía y los enlaces principales.
2. **Habilidades:** presenta las tecnologías y herramientas mediante una lista de iconos.
3. **Proyectos:** utiliza tarjetas para explicar cada proyecto y enlazar su demo y repositorio.
4. **Contacto:** reúne el correo electrónico y los perfiles sociales.

La página principal no necesita JavaScript, una base de datos ni un servidor de aplicaciones. Los enlaces externos abren los recursos publicados, el enlace de correo utiliza el protocolo `mailto:` y el botón del currículum descarga el archivo almacenado en `documents/`.

## Tecnologías utilizadas

- **HTML5:** estructura semántica del contenido.
- **CSS3:** estilos, animaciones, degradados y adaptación de la interfaz.
- **Flexbox:** distribución de elementos en el perfil, los enlaces y las listas.
- **CSS Grid:** organización de las tarjetas de proyectos.
- **Metodología BEM:** nombres de clases organizados por bloque, elemento y modificador.
- **Media queries:** cambios de distribución y tamaño para escritorio, tableta y móvil.
- **Git y GitHub:** control de versiones y alojamiento del repositorio.
- **GitHub Pages:** publicación del sitio estático.

## Decisiones de diseño y desarrollo

- Los estilos están separados por sección para facilitar su lectura y mantenimiento.
- Se utilizan las fuentes locales **Open Sans** y **Archivo Black**, por lo que el diseño no depende de un servicio externo de tipografías.
- Las imágenes usan propiedades como `object-fit` y `aspect-ratio` para conservar una presentación uniforme.
- Los fondos combinan degradados radiales sobre una paleta oscura para dirigir la atención al contenido.
- Las tarjetas incorporan una capa de degradado que mantiene visibles los iconos sobre las imágenes.
- Los enlaces externos usan `target="_blank"` junto con `rel="noopener noreferrer"`.
- La estructura incluye encabezados jerárquicos, textos alternativos y atributos ARIA para mejorar la navegación con tecnologías de asistencia.

## Diseño responsivo

La interfaz parte de una presentación amplia para escritorio y se ajusta mediante dos puntos de cambio:

- **Hasta 1023 px:** reduce tamaños, espacios y convierte la cuadrícula de proyectos en una sola columna.
- **Hasta 767 px:** reorganiza el perfil verticalmente, adapta la fotografía y compacta títulos, enlaces e iconos.

De esta manera, el contenido conserva su jerarquía y legibilidad en pantallas grandes, tabletas y teléfonos.

## Estructura del proyecto

```text
web_project_portfolio_es/
├── documents/              # Currículum descargable en PDF
├── fonts/                  # Fuentes locales en formatos WOFF y WOFF2
├── images/                 # Fotografías, capturas e iconos
├── linkedin-post/          # Material auxiliar para publicaciones de LinkedIn
├── styles/
│   ├── contact.css         # Sección de contacto
│   ├── fonts.css           # Declaración de fuentes locales
│   ├── index.css           # Punto de entrada de los estilos
│   ├── page.css            # Estilos globales y contenedor principal
│   ├── profile.css         # Presentación y enlaces principales
│   ├── projects.css        # Cuadrícula y tarjetas de proyectos
│   └── skills.css          # Lista de habilidades
├── favicon.ico             # Icono del sitio
├── index.html              # Página principal
└── README.md               # Documentación del proyecto
```

## Instalación y ejecución local

El proyecto no requiere instalar dependencias ni ejecutar un proceso de compilación.

1. Clona el repositorio:

   ```bash
   git clone https://github.com/AllenPrkr/web_project_portfolio_es.git
   ```

2. Entra en la carpeta del proyecto:

   ```bash
   cd web_project_portfolio_es
   ```

3. Abre `index.html` en tu navegador.

También puedes utilizar un servidor local, por ejemplo la extensión **Live Server** de Visual Studio Code. Esto permite que el navegador actualice la página con mayor facilidad durante el desarrollo.

## Publicación

El proyecto está publicado con GitHub Pages. Al tratarse de un sitio estático, la plataforma sirve directamente `index.html` y los recursos de las carpetas `styles/`, `images/`, `fonts/` y `documents/`.

## Proyectos mostrados

### Página web de una cafetería

Landing page responsiva desarrollada a partir de un brief de diseño. Incluye estructura semántica, maquetación con Flexbox, secciones informativas y un formulario de contacto.

- [Ver demo](https://allenprkr.github.io/web_project_coffeeshop_es/)
- [Ver repositorio](https://github.com/AllenPrkr/web_project_coffeeshop_es)

### Portafolio personal

Sitio responsivo que reúne mi perfil, habilidades, proyectos y canales de contacto. En este proyecto practiqué la organización modular de CSS, Flexbox, Grid y la metodología BEM.

- [Ver demo](https://allenprkr.github.io/web_project_portfolio_es/)
- [Ver repositorio](https://github.com/AllenPrkr/web_project_portfolio_es)

## Posibles mejoras

- Incorporar nuevos proyectos conforme avance mi formación.
- Agregar filtros para organizar los proyectos por tecnología.
- Implementar un formulario de contacto con validación.
- Añadir un tema claro y permitir que el visitante elija su preferencia.
- Realizar pruebas automatizadas de accesibilidad y rendimiento.

## Autor y contacto

**Luis Alberto Chávez Toussaint**

Desarrollador web junior

- Correo: [luizchavez360@gmail.com](mailto:luizchavez360@gmail.com)
- GitHub: [AllenPrkr](https://github.com/AllenPrkr)
- LinkedIn: [Luis A. Toussaint](https://www.linkedin.com/in/luis-a-toussaint/)
