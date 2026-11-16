# Metodología

## Preparación
Las estructuras se descargan del Protein Data Bank. Se eliminan las moléculas
de agua y los ligandos originales, y se añaden hidrógenos y cargas parciales.
Los inhibidores se descargan de PubChem y se генerа su forma tridimensional.

## Docking
Se usa AutoDock Vina con una caja de búsqueda de 24 x 24 x 24 Å centrada en el
centro activo de cada enzima. Se generan 9 poses por ligando.

## Limitaciones
Ambas enzimas llevan metales en el centro activo (níquel en la ureasa y cobre
en la AMO), que AutoDock Vina describe de forma aproximada. Las energías sirven
para ordenar los compuestos entre sí, no como valores absolutos.
