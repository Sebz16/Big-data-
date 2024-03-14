# Perfilamiento del dataset

## Listado de cambios 
- Se ha eliminado la columna de `Product Page` del conjunto de datos.
- Se ha eliminado la columna de `UPC` del conjunto de datos .
- Se ha aplicado una correcion de formato a la columna de `Length` del conjunto de datos.
- Se ha aplicado una correcion de formato a la columna de `Boost Clock` del conjunto de datos.
- Se ha aplicado una correcion de formato a la columna de `Vram` del conjunto de datos.
- Se ha aplicado una correcion de formato a la columna de `Memory Clock` del conjunto de datos.
- Se ha aplicado una correcion de formato a la columna de `EAN` del conjunto de datos.
- Se ha aplicado una correcion de formato a la columna de `TDP` del conjunto de datos.
## Justificación
- La decisión de eliminar la columna de `Product Page` se basa en la falta de disponibilidad de datos en esta columna y en la baja relevancia de la información para los objetivos de análisis establecidos. La mayoría de los registros contenían valores nulos, lo que indica una falta significativa de información útil.
-  La decisión de eliminar la columna de `UPC` se basa en la falta de disponibilidad de datos en esta columna y en la baja relevancia de la información para los objetivos de análisis establecidos. La mayoría de los registros contenían valores nulos, lo que indica una falta significativa de información útil.
-  La columna `Length` presentaba problemas de formato que afectaban la consistencia y la interpretación de los datos. Estos problemas incluían formatos inconsistentes.
-  La columna `Boost Clock` presentaba problemas de formato que afectaban la consistencia y la interpretación de los datos. Estos problemas incluían formatos inconsistentes, informacion incompleta.
-  
-  La columna `Vram` presentaba problemas de formato que afectaban la consistencia y la interpretación de los datos. Estos problemas incluían formatos inconsistentes.
-  La columna `Memory Clock` presentaba problemas de formato que afectaban la consistencia y la interpretación de los datos. Estos problemas incluían formatos inconsistentes,informacion incompleta.
- - Para la informacion incompleta se opto por utilizar la mediana, para rellenar los datos faltantes debido a la cantidad de datos atipicos que llega al umbral de 10.04%.
-  La columna `EAN` presentaba problemas de formato que afectaban la consistencia y la interpretación de los datos. Estos problemas incluían formatos inconsistentes.
## Impacto del Cambio
- La eliminación de la columna de `Product Page` afectará al análisis de datos que dependía de esta información para identificar los sitios donde se vende el producto. Es importante tener en cuenta que esta acción puede resultar en una pérdida de información sobre los puntos de venta del producto.
- La eliminación de la columna de `UPC` afectará al análisis de datos que dependía de esta información para identificar código de barras. Es importante tener en cuenta que esta acción puede resultar en una pérdida de información para el seguimiento de productos en tiendas.
- La corrección de formato en las columnas `Length`,`Boost Clock`,`Vram`,`Memory Clock`,`EAN` mejoró la calidad y la coherencia de los datos, lo que facilita su interpretación y análisis. Esto asegura que los resultados obtenidos a partir de estos datos sean más confiables y precisos.
## Procedimiento ejecutado
- La eliminación de la columna de `Product Page`.Se llevó a cabo en la hoja de calculo de excel.
- La eliminación de la columna de `UPC`.Se llevó a cabo en la hoja de calculo de excel.
- La correcion de formato de la columna `Length`.Se aplico la formula `VALOR(SUSTITUIR(F2:F1418,"mm",""))` para dejar unicamente los valores numericos en una nueva columna, para reemplazar los datos de la antigua columna con la nueva.
- La correcion de formato de la columna `Boost Clock`.Se aplico la formula `VALOR(SUSTITUIR(N2:N1418,"MHz",""))` para dejar unicamente los valores numericos en una nueva columna, para reemplazar los datos de la antigua columna con la nueva.
- - La insercion de la mediana en la columna de los datos faltantes. Se aplico la siguiente formula `MEDIANA(N2:N1418)`, insertando los datos en las filas con la informacion incompleta.
- La correcion de formato de la columna `Vram`.Se aplico la formula `VALOR(SUSTITUIR(O2:O1418,"MHz",""))` para dejar unicamente los valores numericos en una nueva columna, para reemplazar los datos de la antigua columna con la nueva.
- La correcion de formato de la columna `Memory Clock`.Se aplico la formula `VALOR(SUSTITUIR(P2:P1418,"MHz",""))` para dejar unicamente los valores numericos en una nueva columna, para reemplazar los datos de la antigua columna con la nueva.
- - La insercion de la mediana en la columna de los datos faltantes. Se aplico la siguiente formula `MEDIANA(P2:P1418)`, insertando los datos en las filas con la informacion incompleta.
- La correcion de formato de la columna `EAN`.Se aplico un formato de celda de cientifico a numero.
- La correcion de formato de la columna `TDP`.Se aplico la formula `VALOR(SUSTITUIR(Q2:Q1418,"W",""))` para dejar unicamente los valores numericos en una nueva columna, para reemplazar los datos de la antigua columna con la nueva.
