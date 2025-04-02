# Git lab : Ejercicio

Para este ejercicio he utilizado Visual Studio Code

He empezado creando dos carpetas. Una llamada Repositorio2 y otra dentro de esta llamada "src". Dentro de src , he creado dos archivos llamados index.html e index.js.En ambos archivos lo rellenamos con la documentación dada y hacemos Cntrl + s para guardar los cambios.
[Index html](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/INDEX.png)
[Index js](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/CONSOLE.png)

Fuera de la carpeta src creamos un archivo llamado package.json copiamos la documentación [Package](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/PACKAGE.png)

Una vez que tenemos todo esto abrimos terminal y ejecutamos el NPM Install. Ya instaladas las dependencias, hacemos un NPM START para ver si ha salido todo bien y ver tu página principal subida en el localhost.
[NPM Install y Start](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/NPM%20Install%20y%20start.png)
[Página creada](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/SERVER%20HOST.png)

En la terminal vamos a escribir el comando git init y git status para ver cuales son los ficheros que queremos subir a Github y los que no. [Git init y status](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/.GITIGNORE.png) los ficheros como .parcel-cache , dist, node_modules, package-lock.json no nos interesa tenerlos en el proyecto, asi que para ello creamos un archivo fuera de la carpeta src llamado ".gitignore", en el cual escribimos justo los archivos mencionados antes y guardamos. En el momento de guardar las carpetas pasaran a estar grises indicando que se van a omitir y una vez hacemos git status nos aparecería tal que así [.gitignore](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/GITIGNORE%20.png) reconociendo que .gitignore ha ignorado esos archivos.

Seguimos en la terminal haciendo un "git add ." y un commit -m indicando que es mi primer git inicial. Una vez hecho vamos a la página de Github y creamos un repositorio [Github](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/CREACION%20REPOSITORIO.png). Una vez creada copiamos la dirección SSH [SSH](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/SSH%20REPO.png)

Volvemos a la terminal de nuestro repositorio, vamos a pasar toda la información que tenemos al repositorio creado en la nube. Para ello hacemos un git remote add origin "añadimos la url SSH" y luego hacemos un push -u origin master [Remote y Push](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/COMMIT%20REMOTE%20Y%20PUSH.png)

Habiendo terminado de actualizarse y sincronizar los datos, volvemos a nuestro repositorio en Github y ya si aparecería actualizado tal como lo tenemos en local con las mismas carpetas [Github repositorio](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/REPOSITORIO%20GITHUB.png)

Vamos a jugar ahora con el staging. creamos dos archivos en la carpeta src (temporal y definitivo.txt) [Staging reset](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/RESET%20ESPECIFICO%20Y%20STAGING.png) hacemos un git add . para añadirlo al commit. Aunque aquí solo quiero quedarme con el definitivo el temporal no lo quiero así que hago un reset HEAD especificando el arhivo que quiero pasarlo a Untracked. [restore](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/RESTORE%20Y%20STAGING.png) En esta última foto, he querido hacer un restore para que viesemos si podría volver a como estaba antes de crear estos dos .txt marcando los dos archivos como untracked.

Finalmente como queremos quedarnos con los archivos hacemos un git add . y un git commit -m "jugando con el staging" para finalmente hacerle un push y subirlo a Github. [jugando con el staging](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/COMMIT%20STAGING%20Y%20PUSH.png) [Github staging](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/ARCHIVOS%20SUBIDOS%20GITHUB.png)

Vamos a crear una rama nueva a nuestro repositorio. En la terminal escribimos git branch y el nombre de la rama que queremos crear en este caso "development" luego hemos hecho un git log para ver como se vería en el visual studio code lo que vamos haciendo con las ramas. [Rama development](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/RAMA%20DEVELOPMENT.png)

Nos cambiamos a la nueva rama creada con un git checkout development. Una vez dentro de la nueva rama creamos un fichero en este caso es un index.html con un mensaje. esto lo vamos a guardar y hacer un commit para que veamos las ramificaciones que se van creando. [creando archivos en la rama develompent](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/Captura%20de%20pantalla%202025-04-02%20031449.png)

Vamos a crear otro archivo index.js javascript con un console.log para añadir mas archivos a la nueva rama. Hacemos un git checkout a master y añadimos un .txt ramdom para tener más archivos y que se pueda ver bien las diferencias. [checkout master](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/Creando%20archivos%20javascript%20en%20rama%20nueva.png)

Una vez creado todo volvemos a la rama master para hacer un merge de la rama development sobre la master [merge](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/Creando%20archivos%20javascript%20en%20rama%20nueva.png) y si queremos ver como se vería en el git log [git log merge](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/Merge%20development.png)

Una vez tenemos todo lo que queremos hacemos el git push -u final [push final](https://github.com/Koriox/repositorio2/blob/33a67232b38aa2aaaa058b62cb01b96eee34e81c/Fotos/PUSH%20FINAL%20RAMA%20GITHUB.png) y ya tendriamos el repositorio creado y sincronizado con Github.
