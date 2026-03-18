# Biblioteca Técnica - SVICPDI

Este proyecto contiene la documentación técnica del Soporte del Vicerrectorado de Personal Docente e Investigador (SVICPDI) de la Universidad de La Laguna (ULL).

El sitio está generado con [MkDocs](https://www.mkdocs.org/) y el tema [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/).

## Características

* **MkDocs**: Generador de sitios estáticos rápido y sencillo para documentación.
* **Material for MkDocs**: Un tema moderno y personalizable.
* **Búsqueda integrada**: Funcionalidad de búsqueda en todo el sitio.
* **Navegación mejorada**: Menús automáticos, secciones y pestañas.
* **Gestión de Versiones**: Soporte para múltiples versiones (histórico) mediante [mike](https://github.com/jimporter/mike).
* **Extensiones de Markdown**: Soporte para admonitions, contenido en pestañas, diagramas Mermaid, y más.
* **Optimización**: El sitio final está minificado para un mejor rendimiento.

## Prerrequisitos

* Python 3.x
* Pip (gestor de paquetes de Python)

## Instalación

1. **Clonar el repositorio:**

    ```bash
    git clone <URL-del-repositorio>
    cd tu-proyecto
    ```

2. **Crear y activar un entorno virtual (recomendado):**

    ```bash
    python -m venv .venv
    source .venv/bin/activate  # En Windows: .venv\Scripts\activate
    ```

3. **Instalar las dependencias:**

    ```bash
    pip install -r requirements.txt
    pip install mike
    ```

## Uso

Para iniciar el servidor de desarrollo local con recarga automática:

```bash
mkdocs serve
```

Abre tu navegador y ve a `http://127.0.0.1:8000/`.

## Despliegue

Para generar el sitio estático en la carpeta `site/`:

```bash
mkdocs build
```

## Licencia

Este proyecto está bajo la licencia GNU Affero General Public License v3.0.
