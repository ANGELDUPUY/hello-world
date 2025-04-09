# hello-world
TECNICATURA UNIVERSITARIA EN PROGRAMACIÓN A DISTANCIA
Alumno: Manuel Angel Dupuy
Materia: Programación I
Trabajo Práctico N.º 2: Git y GitHub
Parte 1: Preguntas Teóricas
¿Qué es GitHub?
GitHub es una plataforma de alojamiento de código basada en Git que permite el trabajo
colaborativo en proyectos de desarrollo de software. Ofrece control de versiones, seguimiento
de issues, pull requests y otras herramientas para desarrollo en equipo.
¿Qué es un repositorio remoto?
Un repositorio remoto es una versión del proyecto alojada en un servidor (como GitHub) que
permite la colaboración entre múltiples desarrolladores. Se diferencia del repositorio local que
está en tu computadora.
¿Qué es un fork de repositorio?
Un fork es una copia personal de un repositorio de otro usuario que te permite hacer cambios
sin afectar el proyecto original. Es útil para contribuir a proyectos open source o experimentar
con código ajeno.
Operaciones con repositorios
¿Cómo crear un repositorio en GitHub?
1. Ir a GitHub y hacer clic en "+" → "New repository"
2. Dar nombre al repositorio
3. Elegir visibilidad (público/privado)
4. Opcional: agregar README, .gitignore y licencia
5. Hacer clic en "Create repository"
¿Cómo agregar un repositorio remoto a Git?
git remote add origin https://github.com/usuario/repositorio.git
¿Cómo crear un repositorio privado en GitHub?
Mismo proceso que crear uno público, pero seleccionando "Private" en la opción de visibilidad
durante la creación.
¿Cómo crear un repositorio público en GitHub?
Igual que el privado, pero seleccionando "Public" en la opción de visibilidad.
Ramas (branches)
¿Cómo crear una rama en Git?
git branch nombre-rama Crea la rama
git checkout nombre-rama Cambia a la rama
O en un solo comando:
git checkout -b nombre-rama
¿Cómo cambiar a una rama en Git?
git checkout nombre-rama
O en Git más reciente:
git switch nombre-rama
¿Cómo fusionar ramas en Git?
1. Cambiar a la rama destino (ej: main):
git checkout main
2. Fusionar:
git merge nombre-rama
Commits y cambios
¿Cómo crear un commit en Git?
1. Agregar cambios al staging area:
git add archivo.ext o git add . para todos
2. Crear commit:
git commit -m "Mensaje descriptivo"
¿Cómo enviar un commit a GitHub?
git push origin nombre-rama
¿Cómo empujar cambios a un repositorio remoto?
git push origin nombre-rama
¿Cómo tirar de cambios de un repositorio remoto?
git pull origin nombre-rama
Pull Requests
¿Cómo enviar una solicitud de extracción (pull request) a un repositorio?
1. Hacer fork del repositorio original
2. Clonar tu fork localmente
3. Crear una rama para tus cambios
4. Hacer commits y push a tu fork
5. En GitHub, ir a "Pull requests" → "New pull request"
6. Seleccionar ramas (tus cambios vs original)
7. Describir cambios y crear PR
¿Cómo aceptar una solicitud de extracción?
1. Ir al PR en GitHub
2. Revisar cambios en la pestaña "Files changed"
3. Si todo está bien, hacer clic en "Merge pull request"
4. Confirmar con "Confirm merge"
Etiquetas (tags)
¿Qué es una etiqueta en Git?
Una etiqueta es una referencia estática a un punto específico en el historial, generalmente
usada para marcar versiones (ej: v1.0.0).
¿Cómo crear una etiqueta en Git?
git tag -a v1.0.0 -m "Versión 1.0.0"
¿Cómo enviar una etiqueta a GitHub?
git push origin v1.0.0
O todas las etiquetas:
git push origin --tags
Historial
¿Qué es un historial de Git?
Es el registro completo de todos los commits realizados en un repositorio, mostrando quién hizo
qué cambios y cuándo.
¿Cómo ver el historial de Git?
git log
O con gráfico:
git log --graph --oneline --all
¿Cómo buscar en el historial de Git?
Por mensaje de commit:
git log --grep="texto buscado"
O buscar en cambios de código:
git log -p -S"texto buscado"
¿Cómo borrar el historial de Git?
1. Crear un nuevo commit raíz:
git checkout --orphan nueva-rama
git commit -m "Nuevo inicio"
2. Eliminar la rama original y renombrar esta
Colaboración
¿Cómo invitar a alguien a un repositorio privado en GitHub?
1. Ir a "Settings" → "Collaborators"
2. Hacer clic en "Add people"
3. Ingresar nombre de usuario o email
4. Seleccionar permisos (Read, Write, Admin)
5. Hacer clic en "Add collaborator"
¿Cómo compartir un repositorio público en GitHub?
Los repos públicos son visibles para todos. Puedes compartir el enlace:
https://github.com/usuario/repositorio
