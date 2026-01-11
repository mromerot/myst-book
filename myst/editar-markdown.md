---
title: Editar archivos Markdown
date: 2025-01-10
authors:
  - name: Mauricio Romero T.
    github: mauriciort
exports:
  - format: pdf
---

## Edición de archivos Markdown

MyST permite trabajar principalmente con archivos Markdown (`.md`) para documentos estáticos y Jupyter Notebooks (`.ipynb`) para contenido interactivo con código ejecutable, ambos combinables en un mismo proyecto.

Puede trabajar otros lenguajes de programación en Jupyter Notebooks dentro de archivos (`.ipynb`).

## Pasos para generar un documento Markdown en Myst

1.  **Crear un archivo Markdown**: Comience creando un archivo con extensión `.md` en su proyecto Myst (p.ej. Archivo>Nuevo archivo, en el explorador, etc).
2.  **Agregar el encabezado YML**: Al inicio del archivo, incluya un bloque de encabezado YML con metadatos como título, fecha, autores y opciones de exportación.
  - Complete la mayor cantidad de campos posibles en el encabezado YML para mejorar la organización y presentación del documento.
3.  **Escribir el contenido**: Utilice la sintaxis Markdown para estructurar y formatear el contenido del documento.
4.  **Incluir elementos adicionales**: Puede agregar imágenes, tablas, enlaces y otros elementos multimedia según sea necesario.
5.  **Guardar y compilar**: Guarde el archivo y utilice las herramientas de Myst para compilar y generar el documento final en el formato deseado (PDF, HTML, etc.).  
6. **Incluya el documento en myst.yml**: Debe incluir el archivo en la estructura de la TOC de myst.yml para que sea visible en la plataforma.
7. **Revisión de errores con AI**: Solicite siempre a su asistente de AI que revise la estructura del encabezado .yml y su inclusión en el TOC de myst.yml para evitar errores comunes.

## Encabezado yml

El encabezado YML es una sección especial al inicio de un archivo Markdown que contiene metadatos sobre el documento. En Myst, este encabezado se utiliza para definir propiedades como el título, la fecha, los autores y las opciones de exportación del documento.

### Componentes del encabezado YML

1.  **Título (`title`)**: Define el título del documento. Este título se mostrará en la parte superior del documento y en los índices generados automáticamente.
2.  **Fecha (`date`)**: Indica la fecha de creación o publicación del documento. El formato suele ser AAAA-MM-DD.
3.  **Autores (`authors`)**: Una lista de autores que han contribuido al documento. Cada autor puede tener propiedades adicionales como nombre y perfil de GitHub.
4.  **Exportaciones (`exports`)**: Define los formatos en los que se puede exportar el documento, como PDF, HTML, etc.

| Campo | Descripción |
|----------------|--------------------------------------------------------|
| `title` | Título del documento que aparece en la parte superior y en los índices |
| `subtitle` | Subtítulo opcional para información adicional del documento |
| `short_title` | Versión corta del título para referencias y encabezados |
| `description` | Descripción breve del contenido del documento |
| `date` | Fecha de creación o publicación (formato: AAAA-MM-DD) |
| `authors` | Lista de autores con sus datos (nombre, afiliación, email, etc.) |
| `affiliations` | Instituciones u organizaciones asociadas a los autores |
| `keywords` | Palabras clave para clasificación y búsqueda |
| `license` | Tipo de licencia del documento (ej: CC-BY, MIT) |
| `thumbnail` | Imagen miniatura para representar el documento |
| `banner` | Imagen de banner para la parte superior del documento |
| `tags` | Etiquetas para categorización del contenido |
| `exports` | Formatos de exportación disponibles (PDF, HTML, DOCX, etc.) |
| `bibliography` | Referencias a archivos de bibliografía (.bib) |
| `numbering` | Configuración de numeración de secciones y figuras |
| `math` | Configuración de renderizado de ecuaciones matemáticas |
| `venue` | Información sobre publicación o conferencia |
| `doi` | Digital Object Identifier del documento |