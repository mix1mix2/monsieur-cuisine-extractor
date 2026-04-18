# Monsieur Cuisine Smart - Recipe Extractor

Esta es una microapp diseñada para extraer y visualizar recetas reales directamente desde fuentes externas (web) para tu robot de cocina Monsieur Cuisine Smart.

## ¿Cómo funciona la extracción?

En lugar de guardar recetas fijas, esta app utiliza un **motor de extracción dinámica** basado en:

1.  **Schema.org (JSON-LD)**: La mayoría de sitios web de recetas (incluyendo blogs y sitios oficiales) usan un estándar invisible llamado Schema.org. Esta app lee ese código y extrae automáticamente:
    *   Nombre de la receta
    *   Foto principal
    *   Lista de ingredientes
    *   Pasos de preparación
2.  **CORS Proxy**: Para poder leer sitios externos desde tu navegador, usamos `allorigins.win`, lo que permite "saltar" las restricciones de seguridad y obtener el HTML de la fuente.

## Fuentes recomendadas
*   `monsieur-cuisine.com`
*   `recetasmonsieurcuisine.com`
*   Cualquier blog que use el plugin de recetas de WordPress.

## Instalación
Solo necesitas subir estos archivos a tu **GitHub Pages** para tener tu propio recetario dinámico online.
