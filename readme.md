¡Atención, debes cambiar las credenciales en ConnectionManager para que funcione!


Para ejecutar el springboot desde cmd, debes:

apretar windows+r
ejecutar cmd

ejecutar desde la carpeta de miniproyecto (en este caso):

cd C:/xxxxx

tras abrir la carpeta donde descomprimiste, ejecutar :
mvnw clean package

luego abrir la carpeta target:
cd target 

y luego abrir el java con:
java -jar XXXX.jar 
(XXXX) es nombre de archivo

Y si te sale que tienes un servicio anterior, algo como que ya sea está escuchando el puerto 8080:
netstat -oan -p tcp |find "8080"

Y los ultimos digitos a la derecha serán el XXXX:
taskkill /F /PID XXXX

y volver a abrir el java con :
java -jar XXXX.jar 