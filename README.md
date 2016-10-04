#Ejercicio 1

1. **¿Qué comando utilizaste en el paso 11? ¿Por qué?**	- git reset --hard HEAD~1
	- Porque pediste que perdiéramos los cambios del working copy, luego debíamos obligar a git a borrar dichos cambios dejando los fuentes como estaban en el repo.
2. **¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**	- git reset --hard bd85be501ec54398af4c0aff493e6374f02ed28d
	- Ya que tenía en pantalla el hash de ese commit (había hecho un log justo después de hacer ese commit la primera vez), me resultó lo más rápido y así no dejo commits en el limbo (son baratos, pero se me meten en la cabeza).3. **El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**
	- Un conflicto no, da el mensaje *Already up-to-date.* Entiendo que es porque *styled* va por delante de *master* y no hay bifurcaciones ni commits nuevos, git da por hecho que __*styled* ya incluye a *master*__.4. **El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**
	- Sí, porque tanto *styled* como *htmlify* tienen como padre a *master* y están modificados exactamente en las mismas líneas.

5. **El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**
	- No, porque simplemente hubo que avanzar *master* con fast-forward para absorber *styled*.

6. **¿Qué comando o comandos utilizaste en el paso 25?**
	- git log --graph7. **El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?** 
	- Si podría ser fast-forward porque entre *master* y *title* no hay otros commits que puedan perderse caso de hacer fast-forward.

8. **¿Qué comando o comandos utilizaste en el paso 27?**
	- git reset HEAD~19. **¿Qué comando o comandos utilizaste en el paso 28?**
	- git checkout git-nuestro.md

10. **¿Qué comando o comandos utilizaste en el paso 29?**
	- git branch -D title

11. **¿Qué comando o comandos utilizaste en el paso 30?**
	- git reflog (para obtener el hash del commit del titulo -37604e6-)
	- git checkout 37604e6
	- git checkout -b title
	- git checkout master
	- git merge --no-ff title

12. **¿Qué comando o comandos usaste en el paso 32?**
	- git reset --hard HEAD~313. **¿Qué comando o comandos usaste en el punto 33?**
	- git reflog
	- git reset --hard 2134cdc