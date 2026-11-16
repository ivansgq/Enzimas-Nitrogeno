# Enzimas-Nitrogeno

Estudios de docking molecular en enzimas del ciclo del nitrógeno

Actividad de la asignatura Introducción a la Programación Científica, Máster en Bioinformática.

## Descripción

Cuando se abona un suelo con urea, los microorganismos la transforman en amoniaco (enzima ureasa) y después en nitrato (enzima AMO). Parte del nitrógeno se pierde por el camino, así que en agricultura se añaden productos que frenan estas enzimas.

Este proyecto usa el ordenador para predecir cómo encaja cada inhibidor en el centro activo de cada enzima y compara su afinidad.

## Estructura del repositorio
Carpeta	Contenido:
datos/	Estructuras de las enzimas (PDB) y lista de inhibidores
scripts/	Código del análisis, numerado en orden de ejecución
resultados/	Tablas y figuras que salen del análisis
docs/	Metodología y referencias

Flujo de trabajo:
Descargar las estructuras de las enzimas desde el Protein Data Bank y los inhibidores desde PubChem.
Prepara ambos para el docking (01_preparar.sh).
Acoplar cada inhibidor en el centro activo de cada enzima (02_docking.sh).
Comparar las energías de unión obtenidas (03_analizar.py).

Detalles en docs/metodologia.md.

## Herramientas

AutoDock Vina, AutoDockTools, Open Babel, Python (pandas, Biopython) y ChimeraX para visualizar.

## Organización con Git

El trabajo se dividió en tres ramas, cada una incorporada a main mediante un pull request:

Rama	Qué añade:
datos	Carpeta datos/
scripts	Carpeta scripts/
resultados-docs	Carpetas resultados/ y docs/

Autor
Iván Serrano González
