# Guía de Contribución

## Flujo de trabajo (Trunk-Based Development)
1. Actualizar la rama principal:
   `git pull origin main`
2. Crear una rama de corta duración:
   `git checkout -b feature/nombre-funcionalidad`
3. Realizar los cambios y confirmarlos:
   `git add .`
   `git commit -m "feat: descripción del cambio"`
4. Subir la rama al repositorio remoto:
   `git push origin feature/nombre-funcionalidad`
5. Abrir un Pull Request hacia `main` y solicitar revisión.

## Convención de commits
- feat: nueva funcionalidad
- fix: corrección de errores
- docs: cambios en documentación

## Revisión de Pull Requests
Todo cambio debe ser revisado antes de fusionarse a `main`. `main` es la
rama estable y protegida: no se realizan commits directos sobre ella, todo
cambio ingresa a través de una rama de corta duración y un Pull Request.
