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
```
## Fusionando ramas
Estoy sobre lara ama main y quiero traer lo que esta en features/branch
```sh
git merge <rama-que-quiero-fusionar>
git switch main
git merge features/branch #me traigo a main lo que tenia en features/ramas
```
* fusion -> fast-forward -> git hace la fusion automaticamente
* fusion --> con conflicto -->git no puede fusionar automaticamente, entonces nos va a pedir ayuda a nosotros

## abortar la fusion

```sh
git merge --abort
```

## eliminar una rama
```sh
git branch -d <nombre-rama> # si larama que estoy borrando ya fue fusionada me va a borrar la rama. (aca no genera un commit extra)
git branch -D <nombre-rama> #confirmacion de borrado de una rama que todavia no ha sido fusionada en el repositorio
git branch -d features/branch #ya estaba fusionada features/branch
```


