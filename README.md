# infra-multicapa-SanchezPonce

Vamos a crear una estructura para docker que funcione mediante multicapas y configurar el arranque para evitar posibles fallos.
___
Vamos a necesitar minimo estas 3 capas:
1. una capa de datos que almacene nuestra base de datos y que esta sea persistente y no se borre cuando borremos el contenedor.
2. Una capa Backend que tenga una aplicacion web.
3. Una capa proxy o frontend de un servidor con nginx como proxy inverso que tenga el puerto 80 del host.
