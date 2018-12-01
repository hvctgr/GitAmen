**¿Qué comando utilizaste en el paso 11? ¿Por qué?**  
`git reset --hard HEAD~1`  
Porque si no hicieramos pusieramos el comando --hard se mantendría lo que tengo en mi working copy

**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**  
`git reflog`  
`git reset --hard ID_del_reflog_dondehagocommit`  
Con el reflog vemos los identificadores de todas las operaciones que hemos realizado en nuestro repositorio. 
En él, identificamos el paso anterior al reset y con el reset --hard volvemos a ese estado cambiando el working copy

**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**  
`(styled)git merge master`  
No, debido a que se encuentran en la misma línea de commits.

**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**  
`(htmlify)git checkout styled`  
`(styled)git merge htmlify`  
Causó conflicto porque el archivo git-nuestro.md tiene un contenido diferente en cada rama. Modificamos el archivo para que mantenga los cambios de styled.

**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**  
No, porque se realiza de modo fast-forward. Es decir, está en la misma línea de trabajo de styled.

**¿Qué comando o comandos utilizaste en el paso 25?**  
`git log --all --graph`  
O añadiendo también la opcion --oneline para mostrar menos informacion

**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**  
`(master)git merge --no-ff title`  
Sí, ya que master es padre directo de title.

**¿Qué comando o comandos utilizaste en el paso 27?**  
`git reflog`  
`git reset HEAD~1`  
No utilizo el --hard ya que quiero quedarme con los cambios hechos en el working copy.

**¿Qué comando o comandos utilizaste en el paso 28?**  
`git reflog`    
`git reset --hard ID_del_reflog_delestadoanterior`  
Miro en el reflog el ID de antes del anterior reset y me vuelvo a él.

**¿Qué comando o comandos utilizaste en el paso 29?**  
`git branch -D title`

**¿Qué comando o comandos utilizaste en el paso 30?**  
En el paso 28 al descartar los cambios, entiendo que ya hemos rehecho el merge.

**¿Qué comando o comandos usaste en el paso 32?**  
`git reflog`  
`git checkout ID_inicial`  
Con reflog miro el primer commit realizado, y con el comando checkout muevo el HEAD a esa posicion del arbol.

**¿Qué comando o comandos usaste en el punto 33?**  
`git reflog`  
`git checkout ID_dondeestaelmaster`  
Vuelvo a mirar el reflog y localizo el estado donde estaba por último con el master
