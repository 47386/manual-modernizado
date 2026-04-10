# Manual de Taller Honda Civic — Honda ESM

Manual de Taller electrónico (Honda ESM — Electronic Service Manual) del **Honda Civic 1.8 Sport 2007 (FN2)**, modernizado para funcionar en navegadores actuales.

## Cómo usar el manual

### Opción 1: Abrir directamente (recomendada)

1. Descarga o clona este repositorio en tu equipo.
2. Abre el archivo **`index.html`** con tu navegador web (Chrome, Firefox, Edge o Safari).

> **Nota:** Debido a restricciones de seguridad de los navegadores (`CORS` — Cross-Origin Resource Sharing / `same-origin policy`), el manual funciona mejor cuando se sirve desde un servidor local. Si abres el archivo directamente con `file://` y hay problemas de carga, usa la opción 2.

### Opción 2: Servir con un servidor local

Con **Python** (recomendado):

```bash
# Python 3
python -m http.server 8080

# Luego abre: http://localhost:8080/index.html
```

Con **Node.js**:

```bash
npx serve .
# Luego abre la URL que muestra la terminal
```

### Navegación del manual

1. **Panel izquierdo** — Selecciona el año de modelo y código de modelo. Elige entre *Manual del Taller* o *Manual de Reparación de Carrocería*.
2. **Árbol de sistemas** — Aparece automáticamente tras seleccionar el tipo de manual. Haz clic en una categoría para filtrar los temas.
3. **Botón de búsqueda** (🔍) — Carga la lista de procedimientos filtrados en el área principal.
4. **Área de contenido** — Al hacer clic en un procedimiento, se abre el contenido técnico en una ventana emergente.

## Idiomas disponibles

El manual incluye contenido en los siguientes idiomas:

| Código | Idioma     |
|--------|------------|
| `es`   | Español    |
| `en`   | Inglés     |
| `de`   | Alemán     |
| `it`   | Italiano   |
| `pt`   | Portugués  |

Puedes cambiar el idioma desde la parte inferior del panel de navegación.

## Compatibilidad

Este repositorio ha sido modernizado para ser compatible con navegadores actuales:

| Navegador | Versión mínima |
|-----------|---------------|
| Google Chrome  | 80+ |
| Mozilla Firefox | 75+ |
| Microsoft Edge  | 80+ |
| Safari          | 13+ |

## Archivos originales

Los siguientes archivos son del CD-ROM original y ya **no son necesarios** para usar el manual en un navegador moderno:

- `EsmStart.exe` — Lanzador Windows original (requería Internet Explorer)
- `Autorun.inf` — Configuración de arranque automático del CD-ROM
- `Honda Civic Workshop - Acceso directo.lnk` — Acceso directo de Windows

## Estructura del repositorio

```
├── index.html              ← Punto de entrada moderno (HTML5)
├── HONDAESM.HTML           ← Punto de entrada original (compatibilidad)
├── _COM/                   ← Recursos compartidos (JS, CSS, HTML de cabecera)
├── es/                     ← Contenido en español
│   ├── css/                ← Estilos
│   ├── html/               ← Páginas del manual (~17.000 archivos HTML)
│   ├── img/                ← Imágenes
│   └── js/                 ← Scripts de navegación
├── en/                     ← Contenido en inglés
├── de/                     ← Contenido en alemán
├── it/                     ← Contenido en italiano
└── pt/                     ← Contenido en portugués
```

## Vehículo cubierto

- **Modelo:** Honda Civic 3D / 5D (FN1, FN2, FN3, FN4)
- **Años:** 2007 – 2010
- **Motor:** 1.8 i-VTEC (R18A2)
