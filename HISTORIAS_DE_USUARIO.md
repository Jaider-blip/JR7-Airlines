## Historias de usuario

## HU-01: Ver el menú
Como vendedor de viajes
Quiero ver un menú con las opciones del sistema
Para elegir qué proceso realizar con cada cliente.

- Criterio: el menú muestra las 7 opciones numeradas y vuelve a mostrarse después de cada acción.
- Trazabilidad: RF-01, RF-10

## HU-02: Registrar cliente
Como vendedor de viajes
Quiero registrar nombre, cédula, fecha del viaje y destino del cliente
Para gestionar su plan vacacional.

- Criterio: el sistema solicita los 4 datos y los guarda asociados al mismo cliente.
- Criterio: si la cédula ya existe, avisa y no la duplica.
- Trazabilidad: RF-02, RD-03, RD-04

## HU-03: Seleccionar tipo de maleta
Como vendedor de viajes
Quiero indicar el tipo de maleta con las siglas MB o MP
Para definir el costo base del viaje.

- Criterio: acepta MB, MP, mb y mp. Cualquier otro valor muestra un error y vuelve a pedir el dato.
- Trazabilidad: RF-03, RNF-01, RD-01

## HU-04: Ingresar acompañantes
Como vendedor de viajes
Quiero registrar la cantidad de acompañantes
Para calcular cuántas personas viajan.

- Criterio: acepta enteros mayores o iguales a 0. Texto, decimales o negativos generan un mensaje de error sin cerrar el programa.
- Trazabilidad: RF-04, RNF-02, RNF-06

HU-05: Calcular el valor del viaje
Como vendedor de viajes
Quiero que el sistema calcule el valor total del viaje
Para informar el costo exacto al cliente sin errores manuales.

- Criterio: valor = costo de la maleta × (acompañantes + 1), en COP.
- Criterio: ejemplo: MB con 2 acompañantes = 285.325 × 3 = 855.975 COP.
- Trazabilidad: RF-05, RD-01, RD-02

## HU-06: Visualizar la información
Como vendedor de viajes
Quiero ver todos los datos registrados y el valor del viaje
Para confirmar con el cliente que la información es correcta.

- Criterio: muestra nombre, cédula, fecha, destino, maleta, acompañantes y total.
- Trazabilidad: RF-06

## HU-07: Generar respaldo TXT
Como vendedor de viajes
Quiero guardar la información en un archivo TXT
Para conservar un respaldo de las reservas.

- Criterio: crea el archivo en menos de 5 segundos e informa si se guardó correctamente o si hubo error.
- Trazabilidad: RF-07, RNF-03

## HU-08: Registrar clientes de forma continua
Como vendedor de viajes
Quiero atender varios clientes sin reiniciar el programa
Para agilizar la atención a distintos clientes en una jornada.

- Criterio: al terminar una factura, el sistema queda listo para un cliente nuevo.
- Trazabilidad: RF-08

## HU-09: Terminar la factura con “vacaciones”
Como vendedor de viajes
Quiero escribir la palabra “vacaciones” para cerrar la factura actual
Para pasar al siguiente cliente.

- Criterio: “vacaciones” cierra solo la factura del cliente actual, no el programa.
- Criterio: conviene aceptarla sin distinguir mayúsculas de minúsculas.
- Trazabilidad: RF-09

## HU-10: Salir del sistema
Como vendedor de viajes
Quiero una opción para salir del programa
Para cerrarlo de forma ordenada al terminar la jornada.

- Criterio: la opción 7 finaliza la ejecución.
- Trazabilidad: RF-10
