# Práctica GIT - Respuestas

--

**NOTA:** `[hash]` se refiere a un determinado número que identifica a un cierto punto de modificación de mi repositorio. Por ejemplo, en la pregunta 2 sustituyo `git reset e706023` por `git reset [hash]` para una mejor comprensión.

**1. ¿Qué comando utilizaste en el paso 11? ¿Por qué?**

`git reset --hard HEAD~1` 

Porque con el `HEAD~1` vuelvo atrás 1 cambio y además, usando el `--hard`, descarto mis modificaciones del *working copy*.

--

**2. ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

`git reflog` y `git reset [hash]`

Porque así puedo "restaurar" directamente los cambios que estaban en dicho punto (hash).

--

**3. El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

Ningún problema dado que ambas ramas ya tenían la información actualizada (up-to-date).

--

**4. El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

Este sí generó conflicto, porque el contenido del archivo don-quijote.md de una rama no era el mismo que el de otra, y por tanto, GIT no sabía con cuál quedarse. Lo solventé modificando el archivo directamente.

--

**5. El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

Ningún conflicto. Fue un merge *fast-forward*.

--

**6. ¿Qué comando o comandos utilizaste en el paso 25?**

`git graph`

--

**7. El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Sí,ya que *master* es padre de *title*, por tanto no generaría conflicto.

--

**8. ¿Qué comando o comandos utilizaste en el paso 27?**

`git reset HEAD~1`

Sin utilizar `--hard` conseguimos que los cambios del *working copy* no desaparezcan.

--

**9. ¿Qué comando o comandos utilizaste en el paso 28?**

`git checkout don-quijote.md`

--

**10. ¿Qué comando o comandos utilizaste en el paso 29?**

`git branch -D title`

Utilizando `-D` (en mayúsculas) confirmamos la eliminación.

--

**11. ¿Qué comando o comandos utilizaste en el paso 30?**

`git reflog` y `git reset --hard [hash]`

--

**12. ¿Qué comando o comandos usaste en el paso 32?**

`git checkout [hash]`

--

**13. ¿Qué comando o comandos usaste en el punto 33?**

`git checkout [hash]`