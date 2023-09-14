Creando la version 1.0.0 de este repositorio

### Preguntas sobre Git y GitHub
- ¿Cómo se inicializa un repositorio en Git?

A una carpeta que no tenga su repositorio git lo que hay que hacerle es que una vez descargado Git, se hace click derecho en la carpeta desde el explorador de archivos y se le da click en "Git Bash Here", luego se abre la carpeta en algún editor de código como Visual Studio Code y desde la terminal se escribe "git init" y con eso ya se inicializa el repositorio.

La línea sería la siguiente:

```
git init
```

- ¿Cómo creas un repositorio en GitHub?

Te vas a la página de GitHub, metes tu cuenta o creas una cuenta nueva y desde la página de Home aparece un cuadro que te deja crear un nuevo repositorio 
Sería lasiguiente 


- ¿Cómo vinculas un repositorio local de Git con uno remoto en GitHub?

Una vez hecho el commit de los cambios, para vincular por primera vez el repositorio local con el remoto, primero te aseguras de estar en la rama Main y después se usa el comando "git remote add origin" más el link del repositorio que se tiene en github. Por último, como lo hacemos por primera vez, para hacer el push se debe escribir "git push -u origin main"
```
git branch -M main
git remote add origin https://github.com/usuario/repositorio.git
git push -u origin main
```

- ¿Cuál es el flujo básico de trabajo en Git y GitHub?

El flujo básico de trabajar con git y git hub es que primero se tiene el repositorio local en el que se está trabajando con cambios sin guardar, luego se tiene que hacer "git add" a lo cual se le llama la fase de "Index" o "Staging" la cual guarda todos los cambios y los prepara para subirse al repositorio online, posteriormente cuando se haya varios cambios guardados con git add, se mandan todos ellos en una especie de paquete o conjunto que los contiene todos, el cual se llama commit, para hacerlo se hace con el comando "git commit" (si se quiere agregar un comentario se agrega -m "comentario"). Así cuando se quieran agregar esos paquetes de cambios o commits a la página de github, se hace un git push. Por último, si se hacen cambios en otra computadora o los hace otra persona con acceso al repositorio, entonces para bajar los cambios a la computadora se hace un git pull. 
```
git add .
git commit -m "Comentario"
git push
git pull
```