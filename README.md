# Learning branching  git (Lisbeth Mendoza 2021 1072 - Analisis de sistema)

### Introduccion
- Nivel 1, Realizar un commit "git commit"
- Nivel 2, Crear una nueva rama"git branch bugFix", bugfix es el nombre de tu nueva rama. Para volver a nuevo commit con el nombre de esa rama solo debo usar"git checkout bugfix; git commit"
- Nivel 3, Luego de crear una rama, y crear un commit, volvimos a al commit main "git checkout main" y para poder separar los commit para no tener todo el trabajo ligado "git merge bugfix"
- Nivel 4, hacer rebase. Lo unico diferente de aqui fue hacer rebase "git rebase main" funciona para que dos commit trabajen secuencial aunque esten hechas por separado

### Acelerando
- Nivel 1, head es el commit sobre el cual se esta trabjando, para poder ir a este solo debes escribir "git checkout ´El nombre del commit que estes usando´"
- Nive 2, para ver los hash, que es como la direccion del commit "git log". Para ir al commit atraver de la direccion "tipear 'Los primero 4 digitos'". Para mover 1 commit atras"^" varios "~<num>" 
- Nivel 3, -f reaccina una rama a un commit "git branch -f main" 
- Nivel 4, revertir cambios en git "git reset"->se mueve la rama hacia atras, como si no hubiera existido. "git revert" ->te crea una copia de tu git con los cambios hechos, sin borrar el anterior. 

### Moviendo el trabajo por aqui
- Nivel 1, Copiar commits sobre la ubicacion de HEAD "git cherry-pick <commit 1>" 
- Nivel 2, "pink"-> no poner esto es ignorar la copia de un commit. Para copiar y solo evitar 1 commit debes escribir "git rebase -i HEAD~<num>" 

### Un poco de todo 
 - En los 5 niveles te pedia copiar y organizar los commits de siertas maneras usando los comandos: 
 - Crear una copia y que introduca una rama. "git rebase -i main y git rebase bugfix main"
 - Organizar los comando con "git rebase -i". Para hacer notorio los cambios "git commit --amend" 
 - Se crearon marcas para los commit "git tag v1 c1"
 - Se describio un commit con "git describe" te ayuda a saber donde estabas si te moviste hacia atras o hacia adelante. 
 
 ### Temas Avanzados
 - Fue un repaso de todo lo visto anteriormente
 
 
 # Git Remotes

 ### Push & Pull -- Git Remotes!
 - Nivel 1, Creacion de repositorio remoto "git clone", es creado con una copia del tuyo local. 
 - Nivel 2, para trabajar en el nuevo repositorio remoto se utiliza el comando "git checkout o/main" main es el nomnre de la rama. 
 - Nivel 3, actualiza lo que tienes en tu repositorio local al remoto "git fetch".
 - Nivel 4, "git pull" es como una liga de merge y fetch, clona y separa los commit para que no esten juntos.
 - Nivel 5, "git fakeTeamwork" simula el trabajo de otra persona. Para agregar mas commits con una rama, se utliza el mismo codigo agregando la cantidad de commits "git fakeTeamwork hola 4"
 - Nivel 6, sube los cambios a un repositorio en especifico "git push".
 - Nivel 7, Cuando el repositorio tiene un commit por delate del local no es posible que push se ejecute, lo que se hace es actualizar, organizar el repositorio y ejecutar los cambios. "git fetch; git rebase o/main; git pull"  y alutilizar merge no quiere decir que no mueva el trabajo, dice que integraste los cambios "git fetch; git merge o/main; git pull" y "git pull --rebase; git push" para copiar commit. copia crea y actuliza repositorio. "git pull; git push"
 
 
 
