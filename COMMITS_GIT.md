Para modificar y eliminar commits en Git tanto a nivel local como remoto, hay varias técnicas y comandos que puedes utilizar. Aquí te explicaré algunas de las más comunes junto con ejemplos para ilustrar su uso.

1. Modificar el commit más reciente:
Si deseas hacer cambios en el commit más reciente, puedes usar el comando `--amend`. Esto te permite agregar archivos adicionales, modificar el mensaje del commit o ambos.

```
$ git commit --amend
```

2. Modificar commits anteriores:
Si necesitas modificar commits anteriores, puedes utilizar el comando `rebase` en combinación con la opción `--interactive` o `--rebase` para reescribir la historia de Git. Esto abrirá un editor de texto donde puedes editar los commits.

```
$ git rebase -i HEAD~N
```

Donde `N` es el número de commits anteriores que deseas modificar. Por ejemplo, si deseas modificar los últimos 3 commits, usarías `HEAD~3`.

Una vez que se abra el editor, puedes cambiar `pick` por `edit` en los commits que deseas modificar. Luego, guardar y cerrar el editor. Git pausará en cada commit marcado como `edit`, y puedes realizar los cambios necesarios en cada uno.

3. Eliminar commits locales:
Si deseas eliminar commits locales sin afectar el repositorio remoto, puedes usar el comando `reset`. Elige el tipo de reset que mejor se ajuste a tus necesidades: `soft`, `mixed` o `hard`.

- Soft reset: mantiene los cambios en el área de preparación.
- Mixed reset: deshace los cambios del área de preparación.
- Hard reset: deshace los cambios en el área de preparación y en el directorio de trabajo.

```
$ git reset [--soft | --mixed | --hard] HEAD~N
```

Donde `N` es el número de commits que deseas eliminar.

4. Eliminar commits remotos:
Si necesitas eliminar commits en el repositorio remoto, debes tener en cuenta que reescribir la historia de Git puede causar conflictos si otras personas ya han descargado esos commits. En este caso, es recomendable colaborar con los miembros del equipo y seguir un flujo de trabajo adecuado.

Una forma de eliminar commits remotos es utilizando el comando `push` con la opción `--force` o `-f`. Esto fuerza la actualización del repositorio remoto.

```
$ git push --force origin <branch_name>
```

Sin embargo, debes tener precaución al utilizar `--force`, ya que puede causar problemas si no se usa adecuadamente. Asegúrate de comunicarte con tu equipo y comprender los posibles impactos antes de usar este comando.

Estos son solo algunos ejemplos de cómo modificar y eliminar commits en Git tanto a nivel local como remoto. Recuerda que reescribir la historia de Git puede ser peligroso y puede afectar la colaboración con otros miembros del equipo. Es importante utilizar estas técnicas con precaución y seguir las mejores prácticas de desarrollo colaborativo.
