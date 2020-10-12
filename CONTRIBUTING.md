[English](CONTRIBUTING-en.md)

# Cómo contribuir al H-ART-cktober 2020

- [Restricciones](#restricciones)
- [Registrate en Github](#registrate-en-github)
- [Registrate en el Hacktoberfest](#registrate-en-el-hacktoberfest)
- [Software necesario](#software)
- [Enviando tu arteo, haciendo pull request en este repositorio](#enviando-tu-arte)
- [Recomendaciones adicionales](#recomendaciones-adicionales)

<a name="Restricciones"/>

### Restricciones 

Cada archivo que añadas debe pesar máximo 50 MB.

Todo el material adicional que uses, como tipografía, imágenes u otro, debe tener licencia libre de derechos de autor.

Añade tanto el resultado final como los archivos editables, así como cualquier otro material adicional para su reproducción, como tipografías u otro.

<a name="registrate-en-github"/>

### Registrate en Github 

Para poder hacer pull request es necesario tener una cuenta en Github, para ello ve la página de [registro](https://github.com/join) y sigue los pasos.

**1.- Ingresas tus datos básicos.**

![Image](doc/assets/contributing/github_account/01.jpg)

**2.- Verifica que no eres un robot :robot:.**

![Image](doc/assets/contributing/github_account/02.jpg)

**3.- Presiona el botón de crear cuenta.**

![Image](doc/assets/contributing/github_account/03.jpg)

**4.- Ajustas las configuraciones básicas.**

![Image](doc/assets/contributing/github_account/04.jpg)

![Image](doc/assets/contributing/github_account/05.jpg)

**5.- Revisa tu correo electrónico, y haz click el link que te llegó para verificar tu cuenta.**

![Image](doc/assets/contributing/github_account/06.jpg)

![Image](doc/assets/contributing/github_account/07.jpg)

**6.- ¡Felicidades, ya tienes cuenta en Github! :tada:**

<a name="registrate-en-el-hacktoberfest"/>

### Registrate en el Hacktoberfest 

Para que tus pull request sean tomados en cuenta para el Hacktoberfest, y poder obtener tu franela, debes estar registrado en su [web](https://hacktoberfest.digitalocean.com/); Sigue los pasos para completar tu registro.

**1.- Presiona en el botón Start Hacking**

![Image](doc/assets/contributing/hacktoberfest_register/01.png)

**2.- Inicia sesión en con tu cuenta de Github**

![Image](doc/assets/contributing/hacktoberfest_register/02.png)

![Image](doc/assets/contributing/hacktoberfest_register/03.png)

**3.- Completa el Formulario del Hacktoberfest**

![Image](doc/assets/contributing/hacktoberfest_register/04.png)

**4.- ¡Felicidades, ya estás registrado en el Hacktoberfest! ¡Que comiencen los pull request! :tada:**

![Image](doc/assets/contributing/hacktoberfest_register/05.jpg)

<a name="software"/>

### Software necesario 

Para poder hacer un pull request, es necesario que tengas instalado en tu computadora [Git](https://git-scm.com/).

Después de instalar Git, debes instalar [Git LFS](https://git-lfs.github.com/). 

Opcionalmente, puedes instalar algún cliente gráfico de Git, como [Source Tree](https://www.sourcetreeapp.com/), [Git Kraken](https://www.gitkraken.com/), [GitHub Desktop](https://desktop.github.com/) o algún otro de tu preferencia.

<a name="enviando-tu-arte"/>

### Enviando tu arte o, haciendo pull request en este repositorio

El proceso de hacer un pull request se puede resumir en los siguientes pasos:

- Hacer un fork de del repositorio en Github.
- Hacer un clone del fork en tu computador.
- Configurar tus datos básicos en el clone.
- Crear una rama desde la rama develop.
- Añadir en la carpeta correspondiente, los archivos que quieres enviar.
- Indicarle a git, cuales son los archivos que debe trackear.
- Guardar los cambios en git mediante un commit.
- Sincronizar el fork en Github con un push.
- Y, hacer el pull request al repositorio original desde Github.

A continuación, veremos a más a detalle como hacer cada uno de los pasos del proceso.

**Nota importante: Siempre debes hacer tu pull request contra la rama develop, nunca contra la rama master.**

Empiece haciendo un fork de este repositorio, para ello solo tienes que hacer click en el botón fork en la parte superior derecha.

![Image](doc/assets/contributing/pull_request/00.jpg)

![Image](doc/assets/contributing/pull_request/01.jpg)

Para saber si estás viendo el fork o el repositorio original, fijate en
 la esquina superior izquierda, el título del fork comienza con tu nombre
 de usuario, seguido del nombre del repositorio; además incluye
 el texto **forked from**, con el nombre de usuario y repositorio original.
 
![Image](doc/assets/contributing/pull_request/02.jpg)

A continuación, haz click en el botón verde que dice **code** y copia la URL de la opción HTTPS.

![Image](doc/assets/contributing/pull_request/03.jpg)

Crea una carpeta nueva en tu computador, y abre Git en ella.

![Image](doc/assets/contributing/pull_request/04.jpg)

![Image](doc/assets/contributing/pull_request/05.jpg)

Lo siguiente es clonar el fork del repositorio en la carpeta que creaste. 
 Para ello, en la consola de Git escribe lo siguiente:

`git clone fork_url` 

donde `fork_url` es la URL que copiaste antes; Y presiona enter.

Abre la consola de Git en la carpeta del repositorio que clonaste.

![Image](doc/assets/contributing/pull_request/06.jpg)

Configura Git con tus datos básicos. Primero añade tu dirección de correo eléctronico, escribiendo los siguiente:

`git -config --local user.email "mi_correo@dominio.com"` 

donde `mi_correo@dominio.com` es la dirección de correo eléctronico que usaste para registrarte en Github.
 Luego añade tu nombre escribiendo lo siguiente:

`git -config --local user.name "Nombre y Apellido"`

**Nota: los pasos realizados hasta este punto, solo deben hacerse una vez.
 Todo lo que sigue a partir de aquí, se debe hacer por cada pull request que hagas**

<a name="nuevo-pull"/>

Cambiate a la rama develop, escribiendo lo siguiente:

`git checkout develop`

Crea una nueva rama desde desde la rama develop. Nota: para efectos de ejemplo se usara el nombre *branch_name*.

`git branch branch_name`

Crea una carpeta nueva con tu nombre de usuario en Github, dentro de la carpeta con el día al que corresponde tu contribución, dentro de la carpeta art. Nota: para efectos de ejemplo se usara el nombre *user_name*.

![Image](doc/assets/contributing/pull_request/07.png)

Guarda los archivos correspondientes en la nueva carpeta.
Es recomendable incluir un archivo README.md, donde escribas una pequeña descripción, que programa usar para abrir los editable, así como cualquier otra información que creas pertinente.

Una vez finalices, debes indicarle a Git que haga track de tus archivos, guardar los cambios en Git, y sincronizar los cambios en Github.

Para indicarle a Git que haga track de tus archivos, abre Git en la carpeta donde están los mismo y escribe lo siguiente: 

`git add .` 

y pulsar enter.

Para Guardar los cambios en Git, debes hacer un commit, para ello escribe lo siguiente:

`git commit -m "mensaje"` 

donde `mensaje` es una pequeña descripción de tu aporte.

Para sincronizar los cambios en Github, sólo hace falte hacer un push, para ello escribe lo siguiente:

`git push origin branch_name` 

Ahora sólo hace falta que hagas tu pull request al repositorio original.
Ve al fork del repositorio en Github, allí, busca y selecciona la rama que hiciste push anteriormente.

![Image](doc/assets/contributing/pull_request/08.jpg)

Luego, selecciona la opción **Pull requests**

![Image](doc/assets/contributing/pull_request/09.jpg)

A continuación, pulsa el botón **new pull request**

![Image](doc/assets/contributing/pull_request/10.jpg)

(1) Selecciona el repositorio al que hacer el pull request(comienza con el nombre del otro usuario),
 (2) seguido de la rama a la que quieras hacer el pull request (para este repositorio siempre debes hacer pull request contra la rama develop);
 (3) elige tu repositorio, al que previamente hiciste fork (comienza con tu nombre de usuario),
 (4) y escoge la rama con la que quieres añadir cambios al repositorios principal, es decir, aquella que hiciste push anterioermente.
  
Luego, presiona el botón **create pull request**

![Image](doc/assets/contributing/pull_request/11.jpg)

Debes agregar un título a tú pull request, y opcionalmente puedes añadir una descripción más detallada; Luego presiona el botón **Create pull request**

![Image](doc/assets/contributing/pull_request/12.jpg)

:tada: Si llegaste hasta aqui, es por que ya hiciste tu primer pull request ¡Felicidades! :tada:

![Image](doc/assets/contributing/pull_request/13.jpg)

¿Quieres saber más acercade como se hace un Pull Request? Visita https://www.digitalocean.com/community/tutorials/how-to-create-a-pull-request-on-github

¿Quieres saber más acerca de git? Visita https://git-scm.com/book/es/v2

<a name="recomendaciones-adicionales"/>

# Recomendaciones adicionales

Si tienes alguna duda extra, puedes crear un [Issue](https://github.com/kevinesaa/H-ART-cktober-2020/issues) preguntando cualquier duda que tengas.

- [Creando develop_2](#creando-develop-2)
- [Sincronizando tu fork](#sincronizando-tu-fork)
- [Sincronizando los archivos en tu computador](sincronizando-los-archivos-locales)
- [Antes de hacer otro pull request](#antes-de-hacer-otro-pull-request)

<a name="creando-develop-2"/>

### Creando develop_2

La rama develop_2, es totalmente opcional y sirve para puedas tener todos
 tus creaciones en una única rama, mientras esperas a que tu pull request
 sea integrado al repositorio principal, y luego sincronizar tu fork y el repositorio en tu computador.
 
Abre una consola de Git en la carpeta principal del repositorio en tu computador. 
Luego, cambiate a la rama **develop** escribiendo lo siguiente:

`git checkout develop`

Ahora crea la rama *develop_2*, para ello escribe lo siguiente:

`git branch develop_2`

Para añadir los cambios de otra rama a la rama develop_2, primero debes cambiarte a la misma escribiendo:

`git checkout develop_2`

Y añadimos los cambios de la otra rama mediante un **merge**, de la siguiente forma:

`git merge branch_name`

Todos estos pasos puedes hacerlos después de cada pull request, para mantener todos tus archivos en una única rama.
Además, después de cada *merge* es recomendable borrar la rama que se ha integrado; para ello hacemos lo siguiente:

`git branch -D branch_name`

note que la bandera `-D` debe ser escrita en mayúscula.

Si lo desea, también puede añadir la rama *develop_2* a su fork en Github, escribiendo un push de la forma siguiente:

`git push origin develop_2`

Recuerda que para hacer un push, debes estar en la consola de Git con la
 rama que quieres sincronizar en Github; asegurate de ello
 haciendo `git checkout develop_2` antes.

También es recomendable que borres la rama de tus archivos en Github, luego hacer el pull request, para ello puedes escribir lo siguiente: 

`git push --delete origin branch_name`

<a name="sincronizando-tu-fork"/>

### Sincronizando tu fork

Sincronizar un fork con el repositorio original, es similar a hacer un pull request. Primero, debes ir al fork en Github y buscar la opción pull request.

![Image](doc/assets/contributing/pull_request/09.jpg)

de igual forma, debes presionar el botón **New pull request**

![Image](doc/assets/contributing/pull_request/10.jpg)

Luego, (1) Selecciona el repositorio al que se va a hacer el pull request, en este caso seleccionaras tu repositorio, es decir aquel que comience con tu nombre de usuario.
 (2) Después, debes seleccionar la rama que quieres sincronizar.
 (3) elige el repositorio original, es decir, el que comienza con el nombre del otro usuario.
 (4) y escoge la rama desde donde quieres sincronizar tu repositorio; es recomendable que la rama del paso (2) y del paso (4) sean las misma.

Y presiona el botón **Create pull request**

Nota: si al momento de seleccionar la rama en el paso (2) desapare la opción de elegir el repositorio del paso (3), haz click donde dice **compare across forks**.

![Image](doc/assets/contributing/pull_request/14.jpg)

Aquí también, debes agregar un título a tú pull request, y opcionalmente puedes añadir una descripción más detallada; Luego presiona el botón **Create pull request**

![Image](doc/assets/contributing/pull_request/12.jpg)

Lo anterior, creará una entrada en la sección de pull request de tu fork, buscala y abrela.

![Image](doc/assets/contributing/pull_request/15.jpg)

Ahora, sólo hace falta hacer el merge; Presiona el botón **Merge pull request**, y luego **Confirm merge**.

:tada: ¡Felicidades! si todo está bien ya tines sincronizado tu fork con el repositorio original :tada:

![Image](doc/assets/contributing/pull_request/16.jpg)

<a name="sincronizando-localmente"/>

### Sincronizando los archivos en tu computador

Abre una consola de Git en la carpeta principal del repositorio en tu computador. 
Luego, cambiate a la rama que quieres sincronizar (para este caso se usara la rama **develop**), 
para ello escribe lo siguiente:

`git checkout develop`

Posteriormente, actualizamos la rama de la siguiente forma: 

`git pull`

Y ya con eso tenemos sincronizados los archivos en nuestro computador, de la rama en cuestión.

<a name="antes-de-hacer-otro-pull-request"/>

### Antes de hacer otro pull request

Asegurate de estar en la rama **develop** antes de empezar. Para ello puedes escribir en la consola de Git:

`git checkout develop` 

Si [actualizaste tu fork](#sincronizando-tu-fork), también es recomendable que actualices tus archivos locales. Escribiendo `git pull` puedes asegurarte.

Si lo deseas, puedes borrar la rama donde trabajaste anteriormente, de la forma siguiente:

`git branch -D branch_name`

Opcionalmente, puedes borrar la rama en el fork, escribiendo: 

`git push --delete origin branch_name`

A partir de aquí, sólo tienes que repetir algunos pasos para hacer un
 nuevo pull request, específicamente desde [aquí](#nuevo-pull)
