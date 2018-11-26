## ¿Qué comando utilizaste en el paso 11? ¿Por qué?

git reset --hard HEAD~1

Al utilizar hard, tambien restablecemos lo que habia en el working copy
En head le pasamos despues de ~ 1, para que vaya al anterior.


## ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?

Con git reflog para ver todos los commits.

Luego con git reset --hard y el identificador del ultimo commit, volvemos a donde estabamos antes de desacerlo.
Con este comando el working copy queda igual que como estaba al hacer el hard


## El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

No, porque al hacer el merge, desde la rama styled se pueden acceder a todos los commits de master, incluyendo el que tenia el archivo sin la ultima modificación, psique el ultimo commit contaría ya con todo lo que la rama master podría aportar, cambiaria si se hubiera realizado algún cambio en master después de haber creado la rama


## El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Si
El contenido que había en los archivos eran diferentes en cada rama, ya que ambas partían de master, pero entre ellas no se podia llegar a un commit que tuviera todos los datos.
Al juntarlas, se ha tenido que solucionar el conflicto, en este caso, dejando lo de la rama styled

## El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?

No

Como pasaba en el paso 13, desde la rama styled se puede acceder a los commits de master. En master no se ha modificado nada, por lo cual no hay conflicto.


## ¿Qué comando o comandos utilizaste en el paso 25?

Git log —graph


## El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

No, porque se tiene que realizar un commit después de juntar las ramas.

## ¿Qué comando o comandos utilizaste en el paso 27?

git reset HEAD~1 

## ¿Qué comando o comandos utilizaste en el paso 28?

git commit --amend

## ¿Qué comando o comandos utilizaste en el paso 29? 

Git branch -D title


## ¿Qué comando o comandos utilizaste en el paso 30? 

Git reflog

Git reset —hard 88b9711

Siendo el ultimo pqrametro, el commit donde creábamos el merge
 

## ¿Qué comando o comandos usaste en el paso 32?

Git log, para ver los commits
Git reset —hard y el numero de commit
Para volver al primer commit cambiando el contenido del wordking copy

## ¿Qué comando o comandos usaste en el punto 33?

Git reflog

Git reset —hard y numero

Para volver al ultimo cambio y cambiarlo en el working copy



