## Apuentes para salir de apuros con Git
* Instalamos Git desde cero:
  * winget install --id Git.Git -e --source winget
### Hacemos login o acceso a GitHub.
* Registramos nuestro email:
  * git config --global user.email "you@example.com"
### Carga por primera vez desde nuestro pc a git.
* Inicializamos el repositorio:
  * git init
* Agregamos todos los archivos:
  * git add .
* Creamos el commit, importante indicar que cambio se realizo
  * git commit -m "first commit"
* Creamos y seleccionamos la rama a usar
  * git branch -M main
* Indicamos hacia que repositorio vamos a apuntar:
  * git remote add origin "Aqui ponemos la url de su repositorio, temina en .git"
* Subimos los cambios
  * git push -u origin main
### Carga de cambios
* Agregamos todos los archivos:
  * git add .
* Creamos el commit, importante indicar que cambio se realizo
  * git commit -m "first commit"
* Subimos los cambios
  * git push -u origin main

### Visual Studio Code:
* cannot be loaded because running scripts is disabled on this system. For more information, see about_Execution_Policies at https:/go.microsoft.com/fwlink/?LinkID=135170. + CategoryInfo  SecurityError: (:) [], PSSecurityException + FullyQualifiedErrorId : UnauthorizedAccess
  
Este error es producido por que no tenemos permisos para ejecutar Scripts en PowerShell.
  * Ejecutamos PowerShell en modo administrador y escribimos lo siguiente: Set-ExecutionPolicy Unrestricted
  * Con ello ya deberiamos poder ejecutar correctamente nuestros scripts
