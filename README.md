# git-tbd-actividad

## Descripción
API REST simple para gestionar tareas (`Task`), construida en Java 17 y Spring Boot.
Sirve como proyecto base para practicar Git, GitFlow y Trunk-Based Development
(TBD) en el curso DOY0101 – Ingeniería DevOps. No requiere base de datos: los
datos viven en memoria.

## Instalación
Requisitos:
- Java 17+
- Maven 3.8+ (el proyecto no incluye wrapper, se usa el Maven instalado localmente)

Clonar el repositorio y compilar:
```bash
git clone git@github.com:jhonnylarry/git-tbd-actividad.git
cd git-tbd-actividad
mvn install
```

## Uso
Levantar la aplicación:
```bash
mvn spring-boot:run
```

La API queda disponible en `http://localhost:8080/api/tasks`.

- `GET /api/tasks` → lista las tareas.
- `POST /api/tasks` → crea una tarea (body JSON: `{"titulo": "...", "completada": false}`).

Ejecutar las pruebas:
```bash
mvn test
```

## Estructura de ramas
- `main`: código estable
- `feature/*`: nuevas funcionalidades de corta duración

## Autores
- Jonathan Larraguibel – Desarrollo
