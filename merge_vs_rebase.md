## Merge (Fusión)
El comando `git merge` se utiliza para combinar los cambios de una rama en otra. Al fusionar una rama en otra, se crea un nuevo commit que representa la combinación de ambas ramas. Esto preserva la historia de ambos desarrollos.

📝 Ejemplo en markdown:

Supongamos que tienes dos ramas: `feature` y `main`. Quieres fusionar los cambios de `feature` en `main`. En tu archivo markdown, puedes hacer lo siguiente:

```
Merge feature branch into main branch

Para fusionar los cambios de la rama "feature" en la rama "main", utiliza el comando `git merge`:

1. Cambiate a la rama "main": `git checkout main`
2. Ejecuta el comando de fusión: `git merge feature`
3. Resuelve cualquier conflicto de fusión que pueda surgir.
4. Haz un commit para aplicar la fusión: `git commit -m "Merge feature into main"`

Ahora los cambios de la rama "feature" se han incorporado a la rama "main".
```

```
       A---B---C feature
      /
--1--2--3--4--5 main
            \
             6 merge
```

## Rebase (Reorganización)
El comando `git rebase` se utiliza para reorganizar la historia de los commits en una rama. En lugar de fusionar los cambios, el rebase mueve los commits de una rama a otra, lo que puede proporcionar una historia más lineal y fácil de entender.

📝 Ejemplo en markdown:

Supongamos que tienes dos ramas: `feature` y `main`. Quieres reorganizar la historia de la rama `feature` sobre la rama `main`. En tu archivo markdown, puedes hacer lo siguiente:

```
Rebase feature branch onto main branch

Para reorganizar la historia de la rama "feature" sobre la rama "main", utiliza el comando `git rebase`:

1. Cambiate a la rama "feature": `git checkout feature`
2. Ejecuta el comando de reorganización: `git rebase main`
3. Resuelve cualquier conflicto de reorganización que pueda surgir.
4. Continua con los commits restantes de la rama "feature".
5. Cambiate a la rama "main": `git checkout main`
6. Fusiona la rama "feature" en "main" (opcional): `git merge feature`

Ahora la historia de la rama "feature" se ha reorganizado y se ha colocado sobre la historia de la rama "main".
```
Después de ejecutar estos comandos, los cambios de la rama feature se aplicarán uno por uno sobre la rama main, creando una nueva secuencia de confirmaciones:

```
                   A'--B'--C' feature
                  /
--1--2--3--4--5 main
```

Recuerda que es importante tener cuidado al utilizar el rebase, ya que puede cambiar la historia de los commits y puede causar problemas si la rama ya ha sido compartida con otros colaboradores.
