# Proyecto Megaline
Analizo el comportamiento de los clientes de Megaline para comparar dos tarifas de prepago: Surf y Ultimate. Estudio los datos de 500 usuarios, incluyendo quiénes son, de dónde vienen, qué plan utilizan y cuántas llamadas y mensajes de texto realizaron durante 2018. A partir de estos datos, evalúo qué tarifa genera, en promedio, mayores ingresos y utilizo pruebas estadísticas para determinar qué plan aporta más dinero a la empresa.

1.- Lo primero que se hizo fue una inspeccion y preparacion de datos, esto con el fin de entender la estructura y ver la informacion generalisada.

2.- Despues viendo la informacion a detalle se encontraron algunos errores, columnas con informacion tipo object, fechas que tambien se tenian que convertir a datetime, esto se hizo con el fin de preparar los datos, se convirtieron fechas , aplique el redondo de minutos a la tabla call, se creo una nueva columna con la duracion de cada llamada al minuto entero mas cercano, una ves que las fechas estan en el formato correcto, extrajimos cada registro (llamada, mensaje, sesion) y lo guardamos en una nueva columna month.

3.- El objetivo era calcular el consumo agregado por usuario y por mes. Se añadio una columna clave a cada uno de nuestos dataframes de consumo (calls, messages,internet). Se creo un dataframe consolidado esto con el fin de ver el consumo de cada usuario, para eso se agrego una columna user_id y month.
