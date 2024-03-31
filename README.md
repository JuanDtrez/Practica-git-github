# Practica-git-github

## ¿Qué comando utilizaste en el paso 11? ¿Por qué?
#### Paso 11:
Utilicé el comando `git reset --hard HEAD~1`. Este comando se usa para deshacer el último commit y perder los cambios realizados en el working copy, como indica el ejercicio.

## ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
#### Paso 12:
Usé `git reflog` para encontrar el hash del commit anterior y luego `git reset --hard <hash_del_commit>` para rehacer el último commit que deshice. Esto restauró el commit anterior que habíamos deshecho en el paso 11.

## El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
#### Paso 13:
No, el merge del paso 13 no causó ningún conflicto porque la rama "styled" simplemente absorbió los cambios de la rama "main".

## El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
#### Paso 19:
Podría haber conflictos si se hicieron cambios en las mismas líneas de código en ambas ramas ("styled" y "htmlify"). Se resolvieron quedándose con el contenido de la rama "styled".

## El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
#### Paso 21:
No hubo conflictos porque no había cambios conflictivos entre las ramas "main" y "styled". El merge fue fast-forward, moviendo los commits de "main" hacia adelante hasta el commit de "styled".

## ¿Qué comando o comandos utilizaste en el paso 25?
#### Paso 25:
Usé `git log --graph --oneline --all` para dibujar el diagrama que muestra la estructura del repositorio con todas las ramas y los commits.

## El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
#### Paso 26:
Sí, el merge del paso 26 podría ser fast-forward si la rama "main" no ha tenido cambios desde que se creó la rama "title". En ese caso, "main" avanzaría hasta el commit de "title".

## ¿Qué comando o comandos utilizaste en el paso 27?
#### Paso 27:
Utilicé `git reset --hard HEAD@{1}` para deshacer el merge sin perder los cambios del working copy.

## ¿Qué comando o comandos utilizaste en el paso 28?
#### Paso 28:
Usé `git checkout -- git-nuestro.md` para descartar los cambios en el archivo `git-nuestro.md`.

## ¿Qué comando o comandos utilizaste en el paso 29?
#### Paso 29:
Utilicé `git branch -D title` para eliminar la rama "title".

## ¿Qué comando o comandos utilizaste en el paso 30?
#### Paso 30:
Usé `git reflog` para encontrar el hash del commit del merge deshecho y luego `git reset --hard <hash_del_commit>` para rehacer el merge.

## ¿Qué comando o comandos usaste en el paso 32?
#### Paso 32:
Utilicé `git reflog` para encontrar el hash del commit inicial y luego `git reset --hard <hash_del_commit>` para volver al commit inicial cuando se creó el poema.

## ¿Qué comando o comandos usaste en el punto 33?
#### Paso 33:
Usé `git reflog` para encontrar el hash del commit final y luego `git reset --hard <hash_del_commit>` para volver al estado final cuando se puso título al poema.