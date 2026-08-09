---

# Registro de sesiones

## Sesión 2 – Modularización del proyecto

### Objetivo

Comenzar la transformación de la landing en un proyecto modular para facilitar el mantenimiento y la futura creación de nuevas páginas.

### Trabajo realizado

- Se creó el componente `src/components/Navbar.astro`.
- Se movió todo el HTML del encabezado (`<header>...</header>`) al nuevo componente.
- Se movieron los estilos CSS específicos del Navbar al componente.
- Se importó `Navbar.astro` en `index.astro`.
- Se reemplazó el bloque original del Navbar por `<Navbar />`.
- Se verificó que el sitio siga funcionando correctamente mediante `npm run dev`.
- Se comprendió el funcionamiento básico de los componentes en Astro.

### Estado del proyecto

✅ Navbar modularizado y funcionando correctamente.

## Sesión 3 — Sigue la modularización de componentes

### Navbar
Se extrajo el bloque de navegación de `index.astro` hacia:
`src/components/Navbar.astro`

El componente contiene:
- HTML del Navbar
- CSS específico
- JavaScript del menú móvil

Se eliminó el CSS del Navbar de `index.astro`
y se comprobó que el sitio continúa funcionando correctamente.

### Hero
Se extrajo la sección Hero hacia:
`src/components/Hero.astro`

El componente contiene:
- HTML del Hero
- CSS específico
- Array `zones`, utilizado para generar dinámicamente las zonas mediante `.map()`

En `index.astro` fue reemplazado por:
`<Hero />`

Se eliminó el CSS específico del Hero de `index.astro` y se comprobó que el sitio continúa funcionando correctamente.

###JavaScript del Navbar

Se identificó que el <script> original de index.astro contenía comportamientos correspondientes a distintos componentes.
Este JavaScript fue trasladado a Navbar.astro.

##Responsive

Se detectó que las reglas @media del Navbar permanecían originalmente dentro del CSS de index.astro.

Se trasladaron las reglas correspondientes al Navbar a Navbar.astro.

Esto permitió que el componente sea responsable tanto de su comportamiento en escritorio como de su comportamiento responsive.

Se comprobó el funcionamiento mediante la emulación de un dispositivo móvil de 412 × 915 px.

Resultado:
Navbar de escritorio funciona correctamente.
En móvil aparece el botón hamburguesa.
El menú se abre correctamente.
El botón cambia visualmente a una X.
Los enlaces se muestran correctamente.
Al seleccionar un enlace, el menú se cierra.
El menú ocupa correctamente el espacio debajo del Navbar.
