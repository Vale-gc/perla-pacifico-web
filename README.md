# Festival Perla del Pacífico – Landing page

Proyecto 2: *Explorando la cultura con la web* · Desarrollo de aplicaciones web y móviles (SOFG1006)
Escuela Superior Politécnica del Litoral (ESPOL) · Facultad de Ingeniería en Electricidad y Computación

**Integrantes:** Angel Cedeño · Valeria Gavela
**Estado:** Sprint 1 – Organización del contenido y selección de la plantilla

---

## 1. Descripción del evento

El Festival Perla del Pacífico es un evento cultural y artístico realizado en el Centro Cívico de Guayaquil para conmemorar el 9 de octubre. Participaron flautistas internacionales invitados, que interpretaron obras de Devienne, Magalif y Papadopoulos junto a la Orquesta Sinfónica, bajo la dirección de un director internacional invitado.

**Objetivo del proyecto:** desarrollar una primera versión funcional de una landing page que presente el evento, a partir de la información recopilada durante el levantamiento de datos y de una plantilla HTML y CSS personalizada.

**Justificación:** el sitio acerca la música clásica a la comunidad, difunde la agenda cultural de Guayaquil y proyecta el festival con un estándar profesional, accesible desde cualquier dispositivo.

## 2. Planificación

El trabajo se dividió en tareas pequeñas y se usa GitHub para el control de versiones.

| Tarea | Semana | Sprint |
|---|:-:|:-:|
| Seleccionar el evento y elegir el método de recopilación de datos | 1 | 1 |
| Diseñar la entrevista | 1 | 1 |
| Asistir al evento y recopilar la información | 1 | 1 |
| Organizar contenido y tabla de secciones | 2 | 1 |
| Comparar 3 plantillas de HTML5 UP | 2 | 1 |
| Crear repositorio, README inicial y subir plantilla | 2 | 1 |
| Redactar documentación del reporte | 2 | 1 |
| Personalizar textos e imágenes | 3 | 2 |
| Ajustar colores y estilos (CSS) | 3 | 2 |
| Publicar en GitHub Pages | 3 | 2 |

**Control de versiones**

- `main`: contiene siempre la versión estable del sitio.
- `feature/<tarea>`: una rama por tarea y por integrante (por ejemplo `feature/galeria`).
- Los cambios se integran mediante *pull request* revisado por el otro integrante.
- Commits breves en infinitivo, por ejemplo: `Agregar sección Artistas`.

## 3. Análisis del contenido: secciones del sitio

| Sección | Propósito | Datos que se presentarán |
|---|---|---|
| Inicio (banner) | Captar la atención y dar la información clave del evento | Nombre del festival, fecha (9 de octubre), lugar (Centro Cívico, Guayaquil), frase corta |
| Sobre el festival | Explicar qué es el evento y por qué se realizó | Conmemoración del 9 de octubre, carácter cultural y artístico, objetivo |
| Artistas invitados | Presentar a los flautistas internacionales | Nombre, país de origen y fotografía de cada músico |
| Director y orquesta | Dar a conocer a quien dirigió el concierto y a la Orquesta Sinfónica | Nombre y país del director internacional, reseña breve, fotografía |
| Programa | Mostrar las obras interpretadas y su horario | Obras de Devienne, Magalif y Papadopoulos; horarios y presentaciones |
| Lugar | Ubicar el evento | Centro Cívico, dirección y mapa |
| Galería | Mostrar el evento de forma visual | Fotografías del festival |
| Contacto | Facilitar la comunicación con los organizadores | Correo, redes sociales, formulario |

**Correspondencia con elementos de la plantilla Story**

| Sección | Elemento de Story |
|---|---|
| Inicio | `banner` a pantalla completa con botón ancla |
| Sobre el festival | `spotlight` (texto + imagen) |
| Artistas invitados | `spotlight` alternado o cuadrícula de `items` |
| Director y orquesta | `spotlight` |
| Programa | `items` (tarjetas por obra y horario) |
| Lugar | `spotlight` con mapa incrustado |
| Galería | `gallery` con *lightbox* |
| Contacto | Pie de página con formulario e iconos de redes sociales |

## 4. Comparación de plantillas (HTML5 UP)

Se exploraron las plantillas gratuitas de [HTML5 UP](https://html5up.net/) y se compararon tres candidatas a partir de su código.

| Criterio | Solid State | Hyperspace | **Story** |
|---|---|---|---|
| Estructura | Multipágina (inicio, genérica y elementos). Cabecera fija, banner, 3 spotlights, cuadrícula de tarjetas y pie con formulario | Una página: portada a pantalla completa, 3 spotlights, cuadrícula de 6 características y contacto; incluye página genérica | Una página modular: banner, varios spotlights, galería, cuadrícula de ítems y pie con redes sociales |
| Navegación | Menú hamburguesa con panel superpuesto | Barra lateral con enlaces ancla y desplazamiento suave | Scroll continuo; sin menú en la demo, solo botón ancla en el banner |
| Diseño | «Angular», oscuro y sobrio, imágenes grandes | Bloques de colores, moderno, con animación | Claro y visual, colores de fondo intercambiables y opción de invertir el esquema |
| Adaptabilidad | Responsive, 6 puntos de quiebre (1680 a 360 px) | Responsive, 6 puntos de quiebre; la barra lateral pasa a barra superior | Responsive: escritorio, tablet, tablet vertical y móvil |
| Personalización | Alta | Media-alta | Muy alta: elementos reutilizables con modificadores |
| Ajuste a un evento | Muy bueno | Bueno | Muy bueno |

## 5. Plantilla seleccionada: **Story**

Razones de la elección:

1. Es una landing de una sola página (banner, bloques de contenido y contacto al final), el orden natural para presentar un evento.
2. El banner muestra nombre, fecha y lugar; los *spotlights*, el homenaje al 9 de octubre, los flautistas y el director; los ítems, el programa; y la galería con *lightbox*, las fotografías.
3. Es la más fácil de personalizar: cada sección es un elemento reutilizable que se duplica y se ajusta con clases, muchas veces sin tocar CSS.
4. Es responsive y admite varios colores de fondo y esquema invertido, útil para un tono elegante y cultural.
5. Es gratuita bajo licencia CCA 3.0, con atribución a HTML5 UP.

Por qué se descartaron las otras:

- **Solid State:** está pensada como sitio de varias páginas, innecesario para un solo evento, y su estilo oscuro y sobrio es menos visual para un festival cultural.
- **Hyperspace:** su barra lateral fija reduce el espacio de las fotografías y su estética de bloques de colores encaja menos con un festival cultural.

## 6. Decisiones del sprint

| Aspecto | Decisión |
|---|---|
| Tipo de sitio | Una sola página estática, sin base de datos (el evento ya se realizó) |
| Plantilla | Story (HTML5 UP) |
| Paleta | Tonos sobrios y cálidos (azul del Pacífico y dorado), acordes a un concierto de música clásica |
| Imágenes | Fotografías propias del evento, optimizadas para web |
| Idioma | Español (`lang="es"`) |
| Navegación | Agregar un menú con enlaces ancla, pues la demo no lo incluye |
| Limpieza | Eliminar `index-demo.html` y `assets/js/demo.js`, innecesarios en producción |
| Atribución | Mantener el crédito a HTML5 UP en el pie de página |
| Publicación | GitHub Pages desde la rama `main` |

## 7. Estructura del repositorio

```
perla-del-pacifico/
├── README.md
├── index.html
├── assets/        (css, js, sass, webfonts)
└── images/
```

## 8. Próximos pasos (Sprint 2)

- Reemplazar los textos de demostración por el contenido del festival.
- Sustituir las imágenes por las fotografías del evento.
- Agregar las secciones Director y Programa.
- Ajustar la paleta de colores con las clases de la plantilla.
- Verificar la visualización en escritorio y móvil.
- Publicar en GitHub Pages.

## Créditos y licencia

- Plantilla [Story](https://html5up.net/story) por [@ajlkn](https://html5up.net/), bajo licencia [CCA 3.0](https://html5up.net/license).
- Iconos: Font Awesome. Librerías: jQuery, Scrollex y Responsive Tools (incluidas en la plantilla).
- Imágenes de demostración: Unsplash (CC0), que serán reemplazadas por fotografías del evento.

## Declaración de uso de IA

La IA se utilizó para resumir y traducir el documento entregable a este README. El contenido generado por la misma fue igualmente revisado.