# ifcd0210_desarrollo_web
Certificado de Profesionalidad Desarrollo de Aplicaciones con Tecnologia Web
INSTALACIÓN DE GIT
---------------------
1.instalar Git (control de versiones). https://git-scm.com/ ----->https://git-scm.com/download/win (64-bit Git for Windows Setup.)(Marcar todo los campos )
2.Comprobamos en terminal si tenemos instalado Git correctamente: git --version
Si está bien instalado nos debe aprecer : git version 2.43.0.windows.1, al pulsar enter.
3. Abrir una ventana (sin proyectos). Luego ir a las ... de la barra de herramientas y abrir terminal-> new terminal. Comprobamos que está insatalado git.(usamos el siguiente tutorial).

CREACIÓN DE REPOSITORIO REMOTO - SUBIR ARCHIVOS
------------------------------------------------
1. Abrimos GitHub.
2.Le damos al botón "New" de color verde de la izquierda para crear un repositorio remoto. 
3.Rellenamos los campos con minúsculas y sin símbolos(tildes, comas, etc.): Repository name, Description, le damos a Public, seleccionamos Add a README file, dentro de Add.gitignore buscamos "node"
y le seleccionamos.
4. Por último, le damos a el botón verde del final: Create repository.
5. Entramos en nuestro nuevo repositorio y le damos al botón <> Code.
6. Dentro de code, le damos a la opción HTTPS.
7.Copiamos la url.
8. Nos situamos en la terminal de Visual Studio Code.
Con los comamdos:  cd ..  cd .\Desktop\ (si luego de escribir cd .. colocamos desk y le damos a la tecla tab nos lo autocompleta) nos situamos en el escritorio para clonar la carpeta de nuestro repositorio y tenerla a la vista.
9. Clonamos el nuevo repositorio. Para esto, escribimos en terminal: git clone + url de gitHub, en mi caso:  git clone https://github.com/MHL2022/ifcd0210_desarrollo_web.git, le damos enter y ya tenemos nuestro repositorio clonado en el escritorio. Podemos comprobar que en el escritorio Tenemos una carpeta con el mismo nombre del repositorio de GitHub.
10. Escribimos en terminal (vsc) cd y el nombre de la carpeta clonada, en mi caso: cd .\ifcd0210_desarrollo_web\ (comenzamos a escribir el nombre y con la tecla tab lo autocompletamos).
11. Una vez dentro de la carpeta del repositorio podremos ver el path asi: PS C:\Users\xxxx\Desktop\ifcd0210_desarrollo_web> 
12.Colocamos dentro de la carpeta del repositorio los archivos que queremos subir a GitHub.
13. Escribimos en terminal: git status
14. Podremos ver en terminal el nombre (o los nombres, si son varios) del archivo en color rojo, en mi caso: SubirGithub.txt
15.Escribimos en terminal: git add . y le damos enter.
16.Escribimos en terminal: git status y le damos enter, y veremos el nobre de nuestro archivo en color verde. En mi caso:  new file:   SubirGithub.txt
17. Escribimos en terminal: git commit -m "mi primer archivo" y le damos enter. "mi primer archivo" es el nombre del commit, es solo para identificarlo, si luego hacemos otro commit en la misma carpeta cambiaremos este nombre. 
18. Luego de hacer el commit veremos lo siguiente en terminal: 
*** Please tell me who you are.

Run

  git config --global user.email "you@example.com"
  git config --global user.name "Your Name"
Colocaremos nuestro email con el cual nos registramos en GitHub y nuestro nombre de usuario. Escribiremos(en mi caso): 
git config --global user.email " correo@dominio.com" y le damos enter.
git config --global user.name "MHL2022" y le damos enter.
19. Si tenemos el GitHub abierto, nos saldra una pantalla de validación. Sino lo tenemos abierto nos pedirá que introduzcamos nuestra clave.
20. Reintentamos hacer el commit como en el paso 17, esta vez le cambiamos el nombre, en mi caso:git commit -m "mi segundo archivo" y le damos enter.
21. Hacemos un git satus y le damos enter.
22.Nos saldrá un mensaje que podemos hacer un git push para publicar nuestro local commit.
21. Escribimos en terminal: git push y le damos enter. Ya tendremos subido nuestro archivo, podemos comprobarlo en GitHub.
22. Si hacemos alguna modificación en nuestro archivo y queremos subir el archivo con esta modificación, hacemos: git status (veremos el archivo en color rojo), git add . , git status(veremos el archivo en color verde),  git commit -m "actualizacion"(puede ser cualquier nombre) y por último: git push

