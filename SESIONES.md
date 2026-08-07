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
