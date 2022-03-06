# proyecto
 
•	EC2 - Crear una imagen de una máquina – AMI

vamos a crear con Amazon EC2 imagen builder
Paso 1 crearemos agenda de cuando queremos que se ejecute cuando queramos, pero para demostración usaremos el manual 
 
 
Paso 2 crear una receta
 Una receta de imagen es un documento que define los componentes que se van a aplicar a las imágenes base para crear la configuración deseada para la imagen de salida. Luego de crear la receta, no es posible modificarla. Se debe crear una nueva versión para cambiar los componentes.
 
Se puede escoger entre dos imágenes Linux o Docker 
 
Escogeremos una imagen de origen en este caso en las que la cuenta tenga acceso.
 
Los componentes que usaremos son stig-build-linux-low
 
Usaremos un componente de salida para verificar que la imagen de salida funciona
Simple-boot-test-linux
 
Paso 3 definir la configuración de infraestructura 
Se pueden crear – usar una existente o usar una por defecto en nuestra practica usaremos el por defecto.
 
Paso 4 definir los ajustes de distribución 
 
Paso 5 revisión de todos los datos
 
Vamos a crear 
 
Ahora vamos a generar la imagen 
 
Imagen activa 
 
Creamos una instancia desde imagen AMI
 


•	EC2 - Crear AMI en otra región
 
Instalamos primero httpd- damos star y mandamos un html
 
 
Creamos una imagen
 
 
Creamos una copia de ami con una nueva region
 
 
Lanzamos otra instancia apartir de la ami
 


Comparamos el cambio de región  
1.instancia en norte de virginia  
18.212.5.170 
 
2. instancia California 52.53.202.96

 
 

