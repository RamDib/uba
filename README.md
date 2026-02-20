# Repositorio de Materias CS/Matemática UBA

Este repositorio contiene la estructura y plantillas para organizar tus materias de la facultad.

## Estructura

- **materias/**: Contiene las carpetas de cada materia.
    - **[nombre-materia]/**
        - `notas/`: Tus apuntes en LaTeX.
        - `parciales/`: Enunciados y resoluciones de parciales.
        - `finales/`: Enunciados y resoluciones de finales.
        - `practicas/`: Guías de trabajos prácticos.
        - `recursos/`: Libros, papers, links útiles.
- **utilidades/**: Herramientas compartidas.
    - `latex/`: Plantillas para documentos LaTeX.
        - `structure.tex`: Archivo de estilo principal.
        - `main.tex`: Archivo principal de ejemplo.

## Uso de la Plantilla LaTeX

Para crear nuevas notas para una materia:

1. Copia `utilidades/latex/main.tex` a `materias/[materia]/notas/main.tex`.
2. Edita la línea `\input{structure.tex}` para apuntar correctamente al archivo de estructura.
   - Desde `materias/[materia]/notas/`, el path debería ser `../../../utilidades/latex/structure.tex`.
3. Compila con tu editor de LaTeX preferido (se recomienda `pdflatex` o `lualatex`).
4. Asegúrate de tener instalados los paquetes necesarios (texlive-full o similar).

## Dependencias
- `texlive` (con paquetes `babel`, `fancyhdr`, `tcolorbox`, `listings`, `mathpazo`, etc.)
