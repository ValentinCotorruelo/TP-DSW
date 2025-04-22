# Propuesta TP DSW

## Grupo
### Integrantes
* 52950 - Muntaabski, Felipe
* 53471 - Cotorruelo, Valentín
* 53465- Carbó, Santiago
### Repositorios
* [frontend app](https://github.com/FelipeMuntaabski/Frontend)
* [backend app](https://github.com/FelipeMuntaabski/backtend)


## Tema
### Descripción
Teniamos pensado hacer un sistema para gestionar cocheras en una estacionamiento, con perfiles de administrador y usuario. El administrador puede crear cocheras y modificar las tarifas según el tipo de vehiculo (Auto/Moto) y el tipo de servicio (Anual/Mensual/xHora). Se registrará con la patente al vehículo y el tipo en el sistema el cual calculará las tarifas a abonar. Cualquier servicio que sea fijo, se solicitará dni, nombre, etc al cliente.

### Modelo
![imagen del modelo]()

*Nota*: incluir un link con la imagen de un modelo, puede ser modelo de dominio, diagrama de clases, DER. Si lo prefieren pueden utilizar diagramas con [Mermaid](https://mermaid.js.org) en lugar de imágenes.

## Alcance Funcional 

### Alcance Mínimo

*Nota*: el siguiente es un ejemplo para un grupo de 3 integrantes para un sistema de hotel. El 

Regularidad:
|Req|Detalle|
|:-|:-|
|CRUD simple|1. CRUD Tipo Vehiculo<br>2. CRUD Tipo Servicio<br>3. CRUD Cliente|
|CRUD dependiente|1. CRUD Vehículo {depende de} CRUD Tipo Vehículo <br>2. CRUD Servicio {depende de} CRUD Tipo Servicio|
|Listado<br>+<br>detalle| 1. Listado de cocheras filtrado por tipo de servicio y tipo de vehículo => detalle CRUD Vehículo<br> 2. Listado de clientes filtrado por  fecha hasta el próximo pago de tarifa fija => Muestra tipo de vehículo, patente y tarifa a abonar|
|CUU/Epic|1. Ingresar un vehículo temporal<br>2. Ingresar un vehículo para cochera con tarifa fija|


Adicionales para Aprobación
|Req|Detalle|
|:-|:-|
|CRUD |1. CRUD Vehículo<br>2. CRUD Cochera<br>3. CRUD Localidad<br>4. CRUD Provincia<br>5. CRUD Habitación<br>6. CRUD Empleado<br>7. CRUD Cliente|
|CUU/Epic|1. Reservar una habitación para la estadía<br>2. Realizar el check-in de una reserva<br>3. Realizar el check-out y facturación de estadía y servicios|


### Alcance Adicional Voluntario

*Nota*: El Alcance Adicional Voluntario es opcional, pero ayuda a que la funcionalidad del sistema esté completa y será considerado en la nota en función de su complejidad y esfuerzo.

|Req|Detalle|
|:-|:-|
|Listados |1. Estadía del día filtrado por fecha muestra, cliente, habitaciones y estado <br>2. Reservas filtradas por cliente muestra datos del cliente y de cada reserve fechas, estado cantidad de habitaciones y huespedes|
|CUU/Epic|1. Consumir servicios<br>2. Cancelación de reserva|
|Otros|1. Envío de recordatorio de reserva por email|

