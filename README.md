Documentación del Proyecto CODECATFILMS
Descripción General
El proyecto CODECATFILMS es un sitio web dedicado a la presentación y distribución de contenido multimedia, específicamente series y películas. La interfaz del sitio está diseñada para ser intuitiva y fácil de navegar, permitiendo a los usuarios acceder a diferentes temporadas de series y películas a través de enlaces externos.

Estructura del Proyecto
El proyecto se compone de varios archivos clave que incluyen HTML, CSS, SVG, y JavaScript, organizados en una estructura de directorios que facilita su mantenimiento y escalabilidad.

Archivos Principales
HTML: index.html es el archivo principal que contiene la estructura del sitio web, incluyendo la cabecera, el contenido principal y el pie de página.
CSS: Los estilos del sitio se definen en archivos CSS ubicados en el directorio ./assets/css/, siendo style.css el archivo principal de estilos.
JavaScript: script.js contiene el código JavaScript necesario para la interactividad del sitio, como la funcionalidad del menú de navegación y el botón de regreso al inicio.
Imágenes y SVG: Las imágenes y los iconos vectoriales (SVG) se almacenan en el directorio ./assets/images/. Esto incluye el logo.svg y el favicon.svg.
Funcionalidades Clave
Navegación
El menú de navegación es interactivo y se adapta a dispositivos móviles. Se puede abrir y cerrar mediante botones específicos, cuyos selectores se definen en script.js.

const navOpenBtn = document.querySelector("[data-menu-open-btn]");
const navCloseBtn = document.querySelector("[data-menu-close-btn]");
const navbar = document.querySelector("[data-navbar]");
const overlay = document.querySelector("[data-overlay]");
Efecto de Scroll
El sitio implementa efectos de scroll para mejorar la experiencia del usuario, como cambiar el estilo de la cabecera al desplazarse y mostrar un botón para volver al inicio de la página. Estos efectos se gestionan mediante eventos de scroll en script.js y script.js.

window.addEventListener("scroll", function () {
  window.scrollY >= 10 ? header.classList.add("active") : header.classList.remove("active");
});
window.addEventListener("scroll", function () {
  window.scrollY >= 500 ? goTopBtn.classList.add("active") : goTopBtn.classList.remove("active");
});
Conclusión
El proyecto CODECATFILMS es un ejemplo de cómo se puede crear un sitio web moderno y funcional utilizando tecnologías web estándar. A través de su estructura organizada y código bien documentado, ofrece una base sólida para futuras expansiones o personalizaciones.
