- **¿Que comando utilizaste en el paso 11?. ¿Por qué?**
	$git reset --hard HEAD~1
	Utilizo el hard para perder los cambios, pues es lo que se pide. El
	fichero git-nuestro.md quedará sin los cambios realizados.
- **¿Que comando o comandos utilizaste en el paso 12? ¿Por qué?**
	$git reflog
	(Busco el commit donde añado los cambios al repo, paso 10)
	$git reset --hard ea586f1 (dirección del commit buscado)
	Busco el commit deseado y me desplazo al mismo con el puntero HEAD y
	la rama styled (con checkout solo moveria el puntero head y la rama styled
	se quedaria en el mismo commit que la rama master), modificando el working area. 
	Ahora tengo en el working copy el fichero git-nuestro modificado.
	Con esto Rehago el último commit tal y como se solicita.
- **¿El merge del paso 13 causó algún conflicto? ¿por qué?**
	No causa ningún conflicto ya que se han descartado los cambios al
	deshacer el commit con las variaciones y el fichero git-nuestro.md
	no ha variado.
- **¿El merge del paso 19 causó algún conflicto? ¿Por qué?**
	No porque los cambios realizados en ambas ramas son los mismos y 
	git no detecta diferencias.
- **¿El merge del paso 21 causó algún conflicto? ¿Por qué?**
	Contestar
- **¿Que comando o comandos utilizaste en el paso 27?**
	$git reset HEAD~1
- **¿Que comando o comandos utilizaste en el paso 28?**
	$git checkout git-nuestro.md
- **Que comando o comandos utilizaste en el paso 29?**
	$git branch -D title  (No estando el puntero HEAD en la rama title) 
- **¿Que comando o comandos utilizaste en el paso 30?**
	$git reflog (para buscar el commit donde se añadio el titulo)
	$git merge 1a09af5 (commit buscado antes)
	Lo he hecho fast forward porque el commit del título contiene a master y 
	por tener mas limpio el grafo. Se podia haber hecho tambien $git merge --no-ff 1a091f5 
	y tendriamos un commit mas.
- **¿Que comando o comandos utilizaste en el paso 32?**
	$git reflog
	$git checkout 9cb0613 (commit inicial)
-**¿Que comando o comandos utilizaste en el paso 33?**
	$git reflog
	$git checkout 1a09af5 (commit "Añado título a git-nuestro"


