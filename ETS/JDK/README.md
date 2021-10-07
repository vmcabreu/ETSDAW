# Instalación de JDK en Linux  <a name="id4"></a>
## Índice
- [Creación de la Máquina Virtual](#id1)
- [Instalación de JDK](#id2)
- [Editar la versión de Java predeterminada](#id3)

___
## Creación de la Máquina Virtual <a name="id1"></a>
Para poder proceder a la creación de la máquina virtual necesitaremos el programa **Oracle VM VirtualBox** tras descargarlo e instalarlo empezaremos a crear la máquina virtual.
Tras ejecutar el programa se nos abrirá la interfaz de VirtualBox y el primer paso será crear una nueva máquina virtual pulsando el botón Nueva.
<div align="center">
<img src="Imagenes\Img1.png">
 </div>

Nos saldrá una ventana emergente, la cual nos preguntara que nombre ponerle a nuestra máquina, el directorio donde se instalará y que SO queremos en este caso Linux, Ubuntu.

<img src="Imagenes\Img2.png">

- ### Asignación
El siguiente paso es asignar la cantidad de memoria RAM que queremos usar en la máquina virtual, en mi caso le asigné 2048MB que equivale a 2GB de RAM.

<img src="Imagenes\Img3.png">

Luego le asignaremos un disco duro virtual de unos 10GB de almacenamiento y seleccionaremos de que tipo de disco queremos, en este caso seleccioné el **VDI** (VirtualBox Disk Image) y haremos que el disco solo use el espacio que hay en él a medida que se llene, por lo tanto seleccioné que sea **Reservado dinámicamente**.

<img src="Imagenes\Img4.png"> <img src="Imagenes\Img6.png">

<img src="Imagenes\Img7.png"> <img src="Imagenes\Img8.png">



Con todo configurado ya tendríamos la máquina virtual lista para iniciarla y empezar a trabajar en la instalación de JDK en Ubuntu. Como ven en la imagen, a la derecha, vemos las características de nuestra MV.

<img src="Imagenes\Img9.png">

- ### Inicialización de la MV
Hacemos doble click y la máquina empezará a iniciarse:

<img src="Imagenes\Img10.png">

Nuestra máquina nos pedirá un disco para instalar el SO de Ubuntu, entonces buscamos, descargamos y seleccionamos la .ISO que nos permitira instalar el SO el cual encontramos en la web de [Ubuntu](<https://releases.ubuntu.com/20.04/>). Pulsaremos iniciar y nuestra máquina empezará a moverse e instalar el sistema operativo, por lo tanto habra que esperar un tiempo hasta que lo termine de instalar.
 
<img src="Imagenes\Img11.png" width="400" height="300"> <img src="Imagenes\Img12.png" width="400" height="300">

___
## Instalación de JDK <a name="id2"></a>
Nuestra MV ya ha instalado el sistema operativo y está lista para instalar JDK nuestro primer paso será abrir una terminal

<img src="Imagenes\Img13.png">

Actualizaremos el sistema introduciendo `sudo apt-get update`.

<img src="Imagenes\Img14.png">

Cuando termine de actualizar el sistema, introduciremos `sudo apt-get install default-jdk` para instalar la última versión de Java en la máquina.

<img src="Imagenes\Img15.png">

Introduciremos `S` para confirmar la operación y comenzará la descarga e instalación de archivos.
Cuando termine, comprobaremos la versión de java instalada en nuestro equipo mediante el comando `java -version`, en el que nos mostrará que tenemos la versión 11.0.11

<img src="Imagenes\Img16.png">

Ya que trabajaremos con Java versión 8 tendremos que instalar también esta versión en nuestra máquina.
En este caso realizaremos un `sudo apt install openjdk-8-jdk` en el cual estamos indicando que queremos instalar la versión 8 de Java. Confirmamos la instalación y esperamos.

<img src="Imagenes\Img17.png">

Cuando haya terminado, vemos que tenemos ambas versiones de Java, la 11 y la 8. Pero sigue como predeterminado la versión 11.0.11 entonces debemos cambiar la versión que usará el sistema de forma predeterminada.

<img src="Imagenes\Img18.png">

___
## Editar la versión de Java predeterminada <a name="id3"></a>

Como describimos antes, tenemos la versión 11 de Java como predeterminada en nuestro SO, por lo tanto debemos cambiarlo a la versión con la cual vamos a trabajar que es la 8.

<img src="Imagenes\Img18.png">

Para poder llevar esto a cabo necesitamos introducir el comando `sudo update-alternatives --config java` y esto nos enseñará las versiones de Java que tenemos en nuestra máquina y la que se está usando de manera predeterminada que en ese caso es la 11. Para seleccionar la versión 8 debemos introducir el número `2` y eso hará que Java8 sea el predeterminado.

<img src="Imagenes\Img19.png">

Para comprobar que tenemos la versión que queríamos introducimos el comando 
java -version y como se demuestra en la siguiente imagen, hemos cambiado a la versión 1.8.0

<img src="Imagenes\Img20.png">

___
- [Volver arriba](#id4)
___
- Volver al [índice DAW](<https://github.com/vmcabreu/ETSDAW>)
