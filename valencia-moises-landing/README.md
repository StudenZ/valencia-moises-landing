# Landing Page: Aura Eventos - Producción de Eventos Corporativos y Ferias

## Información del Estudiante
- **Nombre Completo:** Moisés Elías Valencia Ramírez
- **Asignatura:** Fundamentos de Desarrollo Web (Unidad 3)
- **Tema Asignado:** Empresa de producción de eventos corporativos y ferias comerciales
- **Docente:** Ing. Geovanny Brito
- **Institución:** UNIVERSIDAD FUERZAS ARMADAS ESPE

---

## Descripción del Proyecto
**Aura Eventos** es una landing page profesional diseñada para una empresa ficticia de producción y montaje de eventos corporativos, congresos y ferias comerciales. La página comunica la identidad de marca, los servicios de montaje y logística, ofrece paquetes preestablecidos de servicios, recopila testimonios reales de clientes, y posee un formulario dinámico para la cotización de proyectos técnicos de iluminación, audio y estructuras modulares.

El diseño se realizó bajo un enfoque **Mobile-First** utilizando **HTML5 semántico**, **CSS3 modular** (distribuido en 3 archivos independientes), y la grilla responsive de **Bootstrap 5**.

---

## Tecnologías Utilizadas
- **HTML5:** Estructura semántica clara (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`).
- **CSS3 Externo:** Estilos modulares estructurados en 3 archivos.
- **Bootstrap 5 (v5.3.3):** Sistema de rejilla (Grid), espaciados, utilidades de alineación, diseño responsive y componentes interactivos.
- **Bootstrap Icons (v1.11.3):** Biblioteca de iconos vectoriales basada en CSS.
- **Google Fonts:** Fuentes tipográficas de alta calidad (`Outfit` y `Playfair Display`).

---

## Estructura del Proyecto
El proyecto está organizado de la siguiente manera:

```text
valencia-moises-landing/
│
├── index.html            # Estructura de marcado HTML5 y enlazado de recursos
│
├── README.md             # Documentación general y respuestas teóricas del código
│
├── css/                  # Archivos de Estilos Modulares (Mínimo 3)
│   ├── variables.css     # Paleta, fuentes de Google Fonts y tokens de diseño
│   ├── componentes.css   # Estilos para navbar, botones, tarjetas, métricas y formulario
│   └── estilos.css       # Ajustes de secciones, hero, portafolio y consultas de medios
│
├── img/                  # Recursos Gráficos
│   ├── logo.png          # Logo corporativo oficial en colores lavanda y pizarra
│   ├── hero.jpg          # Imagen del escenario principal del hero
│   ├── servicio-01.jpg   # Imagen para el área de Congresos
│   ├── servicio-02.jpg   # Imagen para el área de Lanzamientos
│   └── servicio-03.jpg   # Imagen para el área de Ferias
│
└── docs/                 # Documentos Técnicos
    └── informe.pdf        


```

---

## Variables CSS: ¿Qué son y para qué sirven?

### Definición General
Una **variable CSS** (o propiedad personalizada) es un contenedor dinámico que almacena un valor específico (como un código de color, un tamaño de fuente o una transición) para que pueda ser reutilizado a lo largo de todo el proyecto.

### ¿Para qué sirven?
1. **Mantenibilidad:** Permite centralizar los estilos clave del diseño en un único lugar (`:root`). Si la paleta de colores cambia, solo se modifica en `:root` y la actualización se propaga a todo el sitio web al instante.
2. **Escalabilidad y Organización:** Evita la duplicación constante de códigos hexadecimales o configuraciones tipográficas redundantes en las hojas de estilo.
3. **Consistencia Visual:** Asegura que todos los elementos de la página utilicen exactamente el mismo sistema de diseño.

### Uso en este Proyecto
En la hoja de estilos [variables.css], se configuró la paleta de colores oficial utilizando variables de la siguiente forma:

```css
:root {
    /* Colores Asignados */
    --color-lavanda: #D5CBEA;
    --color-azul-nube: #C5DCEB;
    --color-rosado-frio: #E6CBD8;
    --color-gris-pizarra: #505D6A;

    /* Mapeo Semántico */
    --color-principal: var(--color-gris-pizarra);
    --color-secundario: var(--color-azul-nube);
    --color-acento: var(--color-lavanda);
    --color-resaltado: var(--color-rosado-frio);
}
```

En las demás hojas de estilo (como en `componentes.css` o `estilos.css`), estos colores se aplican dinámicamente mediante la función `var()`:

```css
.btn-custom-primary {
    background-color: var(--color-principal);
    color: var(--color-texto-claro);
}
```

---

## Instrucciones para Abrir la Página Localmente
1. Clona o descarga esta carpeta en tu computadora.
2. Abre la carpeta `landingpage-eventos-valencia-moises`.
3. Haz doble clic en el archivo `index.html` para abrirlo directamente en tu navegador web predeterminado (Chrome, Firefox, Edge, Safari, etc.).
4. Si deseas realizar pruebas en vivo y ver cambios en tiempo real, puedes utilizar la extensión de VS Code **Live Server**.

---

## Fuentes de Imágenes e Iconos
- **Imágenes:** Creadas específicamente para este proyecto utilizando Inteligencia Artificial (herramientas generativas) con el fin de asegurar coherencia visual en colores, estilo fotográfico e identidad corporativa de alta definición, evitando el uso de placeholders vacíos.
- **Iconografía:** Consolidada a través de la biblioteca oficial de **Bootstrap Icons** (v1.11.3). Se representaron los 5 elementos requeridos:
  - **Escenario:** `<i class="bi bi-easel"></i>` (Lanzamientos de Producto)
  - **Calendario:** `<i class="bi bi-calendar-event"></i>` (Planificación / Nosotros)
  - **Micrófono:** `<i class="bi bi-mic"></i>` (Congresos y Convenciones)
  - **Credencial:** `<i class="bi bi-person-badge"></i>` (Ferias Comerciales)
  - **Luces:** `<i class="bi bi-brightness-high"></i>` (Iluminación y Audio)
