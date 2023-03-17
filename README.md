# S learning branching  git (Lisbeth Mendoza 2021 1072 - Analisis de sistema)

### Introduccion
- Nivel 1, Realizar un commit "git commit"
- Nivel 2, Crear una nueva rama"git branch bugFix", bugfix es el nombre de tu nueva rama. Para volver a nuevo commit con el nombre de esa rama solo debo usar"git checkout bugfix; git commit"
- Nivel 3, Luego de crear una rama, y crear un commit, volvimos a al commit main "git checkout main" y para poder separar los commit para no tener todo el trabajo ligado "git merge bugfix"
- Nivel 4, hacer rebase. Lo unico diferente de aqui fue hacer rebase "git rebase main" funciona para que dos commit trabajen secuencial aunque esten hechas por separado

### Acelerando
- Nivel 1, head es el commit sobre el cual se esta trabjando, para poder ir a este solo debes escribir "git checkout ´El nombre del commit que estes usando´"
- Nive 2, para ver los hash, que es como la direccion del commit "git log". Para ir al commit atraver de la direccion "tipear ´Los primero 4 digitos´". Para mover 1 commit atras"^" varios "~<num>" 
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
 
 
