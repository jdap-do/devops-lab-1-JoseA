# DevOps Lab 1 — CI/CD con GitHub Actions y AWS ECS

Aplicación FastAPI que devuelve un saludo personalizado.

## Endpoints

- GET /?first_name=Jose&last_name=Anacona: devuelve un saludo.
- GET /health: devuelve el estado de salud de la aplicación.

## Tecnologías

Python, FastAPI, Poetry, Docker, GitHub Actions y AWS ECR/ECS sobre EC2.

## Objetivo

Automatizar el análisis de código, las pruebas, la construcción y
publicación de la imagen Docker y el despliegue en AWS.

## Flujo de trabajo

Los cambios se realizan en una rama y se proponen mediante un Pull Request
hacia main. GitHub Actions ejecuta Pylint y las pruebas automáticamente.
Al fusionar el Pull Request, el pipeline publica la imagen y despliega en AWS.