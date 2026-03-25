# Biblioteca Técnica - SVICPDI

Este proyecto contiene la documentación técnica del Soporte del Vicerrectorado de Personal Docente e Investigador (SVICPDI) de la Universidad de La Laguna (ULL).

El sitio está generado con [MkDocs](https://www.mkdocs.org/), el tema [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) y gestionado por [mike](https://github.com/jimporter/mike) para el versionado histórico.

## Características

* **Gestión de Versiones**: Histórico de documentación mediante `mike`.
* **Búsqueda integrada**: Funcionalidad de búsqueda avanzada en todo el sitio.
* **Navegación mejorada**: Menús automáticos, secciones y pestañas superiores.
* **Extensiones Pro**: Soporte para avisos (*admonitions*), diagramas Mermaid y contenido colapsable.
* **Optimización**: Minificación automática de activos para una carga rápida.

## Prerrequisitos

* Python 3.x
* Git instalado

## Instalación

1. **Clonar el repositorio:**

    ```bash
    git clone https://github.com/svicpdi/biblioteca-tecnica.git
    cd biblioteca-tecnica
    ```

2. **Entorno virtual y dependencias:**

    ```bash
    python -m venv .venv
    source .venv/bin/activate  # En Windows: .venv\Scripts\activate
    pip install -r requirements.txt
    ```

## Desarrollo y Versiones

A diferencia de MkDocs estándar, el flujo de este proyecto utiliza **mike** para no sobrescribir las versiones anteriores en la rama de despliegue.

### Previsualización local

Para ver cómo queda el manual y el selector de versiones en tu ordenador:

```bash
mike serve
```

Luego abre tu navegador en: `http://localhost:8000/`

### Publicar una nueva versión

Para subir cambios a la web de GitHub Pages (rama gh-pages):

**Si es una versión nueva (ej. v2.0):**

```bash
mike deploy 2.0 latest --update-aliases --push
```

**Si solo quieres corregir algo en la versión actual (ej. v1.0):**

```bash
mike deploy 1.0 latest --update-aliases --push
```

**Para cambiar qué versión se ve por defecto al entrar a la web:**

```bash
mike set-default latest --push
```

## Estructura del Proyecto

* `docs/`: Archivos Markdown (.md) originales que componen la documentación.
* `mkdocs.yml`: Configuración principal del sitio, plugins y extensiones.
* `extra.css`: Estilos CSS personalizados (identidad corporativa ULL).
* `overrides/`: Personalizaciones directas del diseño del tema Material.

## Licencia

Este proyecto está bajo la licencia GNU Affero General Public License v3.0.
