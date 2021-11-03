
# Instalación de Git <a name="id0"></a>

Primero comprobaremos si tenemos Git instalado en nuestro SO, para examinar si está instalado utilizaremos el comando <br>
`git --version`.

<div align="center">
<img src="IMGIT\TeamViewer_PWqeWCciPe.png">
  </div>
  
  ___

Tal y como nos dice la terminal, no encuentra Git, por lo tanto lo tenemos que instalar
mediante `sudo apt install git`.
<div align="center">
<img src="IMGIT\TeamViewer_racfcgnkoM.png">
  </div>
  
Tras terminar comprobaremos que se instaló correctamente con, otra vez, `git --version`
con lo cual nos debería salir la versión más reciente que sería la 2.25.1.
<div align="center">
<img src="IMGIT\TeamViewer_DtUpyesU18.png">
  </div>
  
___
##Configuración Git
Tras la instalación de Git lo tendremos que configurar mediante el comando `gitconfig`. En
este caso queremos configurar nombre y email, entonces usaremos `gitcofig --global
user.name “Nombre”` y `gitcofig --global user.email “Correo electrónico”` para añadir estos
dos campos a la configuración de Git.
<div align="center">
<img src="IMGIT\X2DUkEvAs4.png">
  </div>
  
  Dado que el terminal no nos dice nada, suponemos que lo hemos hecho bien pero para
asegurarnos, entraremos al archivo de configuración de Git con `nano ~/.gitconfig`.
<div align="center">
<img src="IMGIT\TeamViewer_xHe38bUkup.png">
  </div>
  
  Tal como nos muestra Nano hemos añadido nuestros dos campos con éxito, tan solo
tendremos que salir de nano con Ctrl+X y tendríamos instalado Git en nuestro sistema.

___
- [Volver arriba](#id0)

___
- Volver al [índice DAW](<https://github.com/vmcabreu/ETSDAW>)
