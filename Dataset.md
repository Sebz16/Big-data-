# Perfilamiento del dataset

## Listado de cambios 
- Se ha eliminado la columna de `Product Page` del conjunto de datos.
- Se ha eliminado la columna de `UPC` del conjunto de datos .
- Se ha aplicado una correcion de formato a la columna de `Length` del conjunto de datos.
- Se ha aplicado una correcion de formato a la columna de `Boost Clock` del conjunto de datos.
- Se ha aplicado una correcion de formato a la columna de `Vram` del conjunto de datos.
- Se ha aplicado una correcion de formato a la columna de `Memory Clock` del conjunto de datos.
- Se ha aplicado una correcion de formato a la columna de `EAN` del conjunto de datos.
## Justificación
- La decisión de eliminar la columna de `Product Page` se basa en la falta de disponibilidad de datos en esta columna y en la baja relevancia de la información para los objetivos de análisis establecidos. La mayoría de los registros contenían valores nulos, lo que indica una falta significativa de información útil.
-  La decisión de eliminar la columna de `UPC` se basa en la falta de disponibilidad de datos en esta columna y en la baja relevancia de la información para los objetivos de análisis establecidos. La mayoría de los registros contenían valores nulos, lo que indica una falta significativa de información útil.

## Impacto del Cambio
- La eliminación de la columna de `Product Page` afectará al análisis de datos que dependía de esta información para identificar los sitios donde se vende el producto. Es importante tener en cuenta que esta acción puede resultar en una pérdida de información sobre los puntos de venta del producto.
- La eliminación de la columna de `UPC` afectará al análisis de datos que dependía de esta información para identificar código de barras. Es importante tener en cuenta que esta acción puede resultar en una pérdida de información para el seguimiento de productos en tiendas.

## Proceso de Eliminación
- La eliminación de la columna de `Product Page` se llevó a cabo utilizando la hoja de calculo de excel. Para eliminar la columna del conjunto de datos original.
- La eliminación de la columna de `UPC` se llevó a cabo utilizando la hoja de calculo de excel. Para eliminar la columna del conjunto de datos original.
