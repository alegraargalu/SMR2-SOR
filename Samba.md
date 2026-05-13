## Tarea 1: Clasificación de Roles de Seguridad
### Aquí vamos a gestionar el poder que tendrán las cuentas en el sistema del hotel.
```mermaid
flowchart TD
A[Las cuentas de los ordenadores para los huéspedesa tendrán el rol Nivel 0, con este rol no pueden acceder a ninguna información del sistema ni modificar nada, pero si utilizar el equipo y estar bajo la protección de la infraestructura lógica del hotel.]
A-->B[Los empleados de limpieza tendrán el rol Nivel 0, con este rol solo podrán ver cuando los huéspedes se han ido o el empleado puede ir a limpiar la habitación.]
B-->C[A los empleados encargados de llevar pedidos o encargos a las habitaciones de los huéspedes se les pondrá el rol de Nivel 2, con este rol tiene accsso a las carpetas dónde pone los datos de los huésppedes, número de habitación, nombre y apellidos, cosas de este estilo, pero con más permisos que los empleados de Nivel 1.]
c-->D[A los empleados del departamento de contabilidad se les asigna el Nivel 3, con  este nivel tiene acceso a todos los archivos y carpetas con los datos de ingresos y gastos.]
D-->E[Gerente, a este se le pone el nivel más alto de emppleados, Nivel 4, con este nivel tiene acceso a todos los archivos de todas las carpetas.]
E-->F[El último nivel que queda es el Nivel 5, este nivel no se le puede dar a ningún empleado, sino que, es el nivel para el dueño de todo el hotel si quiere estar activo en el sistema, pero puede no existir.]
```

## Tarea 2: Inventario y Planificación de Recursos
Para el hotel se necesitarán ordenadores según el número de empleados y habitaciones, por cada habitación un ordenador, y luego por cada empleado un ordenador y si es un empleado que tiene que estar en constante movimiento por el hotel una tablet que, o esté vinculada al ordenador de ese empleado que va a ejecutar los procesos o que la misma tablet esté en la estructura del sistema. Además habrá una impresora por cada empleado que esté en oficina, que no se esté moviendo durante todo el día.
