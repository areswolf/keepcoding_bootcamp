# Preguntas y respuestas
####- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
git reset --hard HEAD~1
De este modo vuelvo al *commit* anterior con el modificador *--hard* que me cambia el working copy

####- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
Primero localicé el *commit* nº2 con *git reflog*, y vi que era el *55576fa*. Después, hice *git reset --hard 55576fa*, que me reposiciona los punteros en ese *commit* y me cambia el *working copy* (por el atributo *--hard*)

####- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
######NOTA: En este paso, entiendo que es *styled* quien absobe a *master* (no "htmlify").
No causa conflicto, porque tras el merge, está "up-to-date".
 
####- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
Sí, causó conflictos porque el "mergeo" pretende mezclar todas las líneas coincidentes en ramas "paralelas", y hay que decidir con cuál de los dos nos quedamos en la "mezcla"

####- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
No, porque styled ya se había comido a master varios pasos antes, no hay ramas paralelas y por tanto no hay lineas que coincidan en la mezcla. Es un merge FF.

####- ¿Qué comando o comandos utilizaste en el paso 25?
*git log --graph --decorate --pretty=oneline*

####- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué? 
*git merge --no-ff title*. Sí, sin problema, pues valdría con avanzar los punteros.

####- ¿Qué comando o comandos utilizaste en el paso 27?
*git reset f8da58b*

####- ¿Qué comando o comandos utilizaste en el paso 28?
*git reset --hard HEAD*

####- ¿Qué comando o comandos utilizaste en el paso 29?
*git branch -D title*

####- ¿Qué comando o comandos utilizaste en el paso 30?
*git reset --hard abc44c0* (después de ver la referencia con *reflog*)

####- ¿Qué comando o comandos usaste en el paso 32?
*git reflog*

*git reset --hard 43db34e*

####- ¿Qué comando o comandos usaste en el punto 33?
*git reflog*

*git reset --hard f8da58b*

