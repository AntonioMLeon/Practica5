# Practica5

Primero hemos creado nuestro repositorio **“Practica5”** en GitHub y lo hemos clonado en nuestra máquina local.

Creamos el archivo **gitignore** y ignoramos el **.env** y cambiamos nuesrtras configuraciones para provocar errores.

Para trabajar con el flujo de GitFlow usamos el siguiente comando:
```
git flow init
```
Ahora creamos las ramas con nuestros nombres:
```
git branch "feature/Tony"
```
Y la rama develop:
```
git branch "develop"
```
y hacemos un push:
```
git push origin "feature/Tony"
git push origin "develop"
```
Agregamos contenido personalizado al archivo index.html. En el index tienen
que aparecer vuestros datos personales mostrados en la web (DNI, Nombre,
Apellidos):

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <p><b>DNI:</b>29547311Q</p>
    <p><b>Nombre:</b>Antonio</p>
    <p><b>Apellidos:</b>León Jiménez</p>
</body>
</html>
```
Hacemos commits y empujamos las ramas al repositorio remoto y entramos en la rama develop y hacemos un merge:
```
git checkout develop
git merge feature/Tony
```
Ahora hacemos un release de versión:
```
git flow release finish 0.1
git flow release finish 0.2
```
Nos metemos en la rama de main y iniciamos un hotfix:
```
git checkout main
git flow hotfix start hotfix/tony
```



