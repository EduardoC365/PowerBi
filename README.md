# PowerBi
Estos son los pasos a seguir para conectar Hadoop + YARN + Hive + PowerBI.
Para hacer este proceso tienes que ejecutar la imagen y desplegar el contenedor de docker del repositoro de docker-hive donde estan los archivos necesarios para poder hacer esta tarea. Tendremos que tener el contenedor de hive activo.

## Primer paso: Instalación
Descargamos Power Bi Desktop desde la tienda de microsoft. Instalamos la aplicaión y accedemos a ella.

##Segundo paso: Configuración de Power Bi
Ya dentro de la aplicación aceptamos tomo como viene por defecto.
Entramos en la pagima principal y damos a la sección de obtener datos de otros orígenes, damos a otras bases de daros y seleccionamos Hive LLAP y le damos a conectar

## Hive LLAP
Donde pone servidor ponemos localhost:10000, en base de datos ponemos default y protocolo de transporte Thrift le damos estádar. En modo conectividad lo dejamos en Importar.

##Conectar el servidor
Nombre de usuario es root y contraseña root. Le damos aceptar al aviso.

##Pasos finales
Seleccionamos la base de datos que queremos cargar en este cosa la mia es pokes y le damos a cargar.
Ya tienes hive conectado con power bi.

##Mini prueba 
En la derecha en datos desplegamos la tabla pokes en mi caso y arrastamos los datos en un grafico para poder ver los datos de nuestra tabla.
