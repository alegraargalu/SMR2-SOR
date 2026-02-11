# Instalación, configuración y uso de OpenLDAP
## Previo a instalar OpenLDAP
Antes de ponernos a instalar el OpenLDAP, pero ya con la máquina ubuntu sin interfaz gráfica, tendremos que hacer la configuración de la dirección IP de nuestra máquina, la máquina, como mínimo, tiene que tener un adaptador, cuando ya estés en la línea de comandos ,ejecuta el siguiente comando: sudo nano /etc/netplan/50-cloud-init.yaml. Y cuando estés dentro de ese fichero, escribe lo siguiente.
<img width="1920" height="1080" alt="imagen" src="https://github.com/user-attachments/assets/e49c9d80-be8c-4bf5-b88d-5372f11a8b16" />
Después de haber hecho esto, pulta "control + X", luego "y" y por último "enter". Después de pulsar estos botones en ese orden en la línea de comando escribe "sudo netplan apply" y comprueba si ha sido efectiva la modificación con "ip address". Si los cambios no se han efectuado prueba a reiniciarlo con "sudo reboot", y ya deberían de haberse hecho los cambios, si no es así revise el fichero netplan, y si nada de esto funciona, probablemente su máquina este corrupta.



## Instalación
Para realizar la instalación primero ejecutaremos "audo apt update" para actualizar el sistema, después de que haya acabado la actualización ejecutaremos "sudo apt install slapd ldap-utils", con este comando instalaremos el OpenLDAP. Después de ejecutar el comando aparecerá la siguiente pantalla:
<img width="1920" height="1080" alt="imagen" src="https://github.com/user-attachments/assets/8ba78e1b-7c5f-4a11-b973-6b030ce72a2e" />
Aquí pondrás la contraseña que quieras, mi recomendación es que pongas la misma que tienes para ingresar en la cuenta de administrador.



## Configuración
Ahora para configurar el slapd, ejecutamos el comando "sudo dpkg-reconfigure slapd", al ejecutar el comando aparecerá la siguiente pantalla preguntándonos si queremos omitir la configuración de slapd, elegiremos que No.
<img width="1920" height="1080" alt="imagen" src="https://github.com/user-attachments/assets/4a139128-b398-41ee-b51d-12a785b56cb7" />

Luego eliges el nombre que quieres que tenga tu dominio.
<img width="1920" height="1080" alt="imagen" src="https://github.com/user-attachments/assets/41b5313b-434e-417e-9478-22df45f71ab1" />

También el nombre de organización.
<img width="1920" height="1080" alt="imagen" src="https://github.com/user-attachments/assets/cdb16bb2-99c1-4247-a015-c9f721844153" />
