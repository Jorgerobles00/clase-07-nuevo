# GIT RAMAS (Branches)

## Crear un repositorio

```sh
git init
```

## Ver el status de los archivos 

```sh
git status
```

## Git alias Alias...

```sh
git config --global alias.st "status --short"
git config --global alias.a "add"
git config --global alias.c "commit -m"
git config --global alias.l "log --oneline"
```
 
## Ver las direrencias en el WD y el LR

```sh
git diff
```

## ver el contenido de cada commit 
``` sh
git show <numero-hash>
```
## crear una rama

```sh
git branch <nombre-rama> #crea una rama y nos deja en la rama actual
git branch features/ramas
git switch -c <nombre-rama> #crea una rama y nos mueve a la rama que se creo
```

## Me muevo entre ramas
```sh
git switch <nombre-rama>
git switch features/ramas
```

## Comparar entre los ultimos commits de las ramas

```sh
git diff <nombre-rama-que-quiero-comparar> #comparo la arama actual contra la rama que indico
git diff dev # ejemplo, comparo features/ramas con dev
```
## Ver las ramas locales y remotas
```sh
git branch -a #Me muestra las ramas locales y remotas


