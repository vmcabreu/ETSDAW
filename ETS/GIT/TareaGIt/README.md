<div align="justify">
  
# Tareas Básicas GIT
## Índice
- [Configuración](#id1)
- [Creación de un repositorio](#id2)
- [Comprobar el estado del repositorio](#id3)
- [Realizando COMMIT](#id4)
- [Modificación de ficheros](#id5)
- [Historial](#id6)

## Configuración <a name="id1"></a>
  Primero comenzaremos a configurar nuestro GIT, en este caso añadiremos un nombre de usuario y un correo electrónico con los comandos:
```  
git config --global user.name "Nombre de usuario" 
git config --global user.email "Email"
```
Luego modificaremos el color de la interfaz en automático mediante `git config --global color.ui auto`.
Para comprobar que hemos realizado todo bien ejecutaremos un `git config --list` para ver que datos hemos añadido a nuestra configuración de git.
  
<div align="center">
<img src="IMGIT\IMG1.png">
  </div>

## Creación de un repositorio <a name="id2"></a>
  Tras configurar git crearemos una carpeta llamada dpl mediante el comando `mkdir (make directory)` y abrimos esa carpeta con  
  `cd (change directory) dpl`. 
Luego ejecutaremos `git init` para inicializar un repositorio Git dentro de la carpeta y para comprobarlo usamos `ls -la` para ver el contenido de la carpeta confirmando que tenemos un .git dentro de ella
  <div align="center">
<img src="IMGIT\IMG2.png">
  </div>
  
## Comprobar el estado del repositorio <a name="id3"></a>
Ya creado, comprobaremos el estado del repositorio  con `git status`. Luego crearemos un archivo indice.txt  con el comando `cat >` y lo añadiremos al git mediante `git add indice.txt`.
Tras este último paso comprobaremos nuevamente el estado del repositorio con `git status`.
  <div align="center">
<img src="IMGIT\IMG4.png">
<img src="IMGIT\IMG5.png">
  </div>
  
## Realizando COMMIT <a name="id4"></a>
  Realizaremos un `git commit -m` para añadir los cambios al repositorio y luego comprobaremos el estado del git de nuevo con `git status`.
    <div align="center">
<img src="IMGIT\IMG6.png">
  </div>

## Modificación de ficheros <a name="id5"></a>
  Para modificar en este caso nuestro índice dentro del repositorio usaremos de nuevo el comando `cat > indice.txt` para editarlo.
Añadimos o editamos la información y lo guardamos para ver qué cambios hemos hecho realizaremos un `git diff`, para ver lo que se ha editado.
Volvemos a añadir nuestro archivo modificado mediante `git add` y realizaremos un `git commit -m`, documentando los cambios recibidos.
    <div align="center">
<img src="IMGIT\IMG7.png">
<img src="IMGIT\IMG8.png">
  </div>
  
## Historial <a name="id6"></a>
  Podremos comprobar el historial de los cambios que se han realizado en el repositorio con 
`git show`.
Dado que se me ha olvidado añadir algo al commit anterior, lo arreglaremos ejecutando 
`git commit --amend -m` y editaré el antiguo commit.
Tras terminar usare otra vez `git show` para ver si se ha cambiado con éxito.
    <div align="center">
<img src="IMGIT\IMG9.png">
<img src="IMGIT\IMG10.png">
<img src="IMGIT\IMG11.png">
  </div>
  
  
</div>
