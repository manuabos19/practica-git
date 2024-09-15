- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
 git reset --hard HEAD~1 - Este comando sirve para mover el puntero de la rama en la que estas a otro commit especificado con "1" desahciendo los cambios al directorio, con el añadido de HARD los borra por completo 
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
git reflog - git reset --hard 7c0b474 . Primero utilice el git reflog para saber el hash del commit, me situe en la rama styled y realice un reset hard al hash del commit. Esto devolvio la rama al commit borrado. 
- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
git merge main (Already up to date.) - No causa conflicto porque los cambios ya se encuentran en la rama styled
- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Si lo causa porque el contenido de ambos es diferente y coincide en las mismas lineas. He tenido que acceder al archivo para resolverlo, quedandome con los datos de styled
- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
No causa conflicto, actualiza los datos de la rama main realizando un fast-forward entre las dos ramas al no existir mas commit desde la rama main simplemente se actualizan
- ¿Qué comando o comandos utilizaste en el paso 25?
git log --oneline --graph --all --decorate
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
No, porque ya existen mas commit desde la rama main que no pertenece a la rama title
- ¿Qué comando o comandos utilizaste en el paso 27?
git reset HEAD~1
- ¿Qué comando o comandos utilizaste en el paso 28?
git restore git-nuestro.md
- ¿Qué comando o comandos utilizaste en el paso 29?
git branch -D title
- ¿Qué comando o comandos utilizaste en el paso 30?
git reflog - git reset ec7a61f
- ¿Qué comando o comandos usaste en el paso 32?
git reflog -  git checkout 366ab75
- ¿Qué comando o comandos usaste en el punto 33?
git reflog - git checkout ad30942
