# Backend del Proyecto – FastAPI

## Instalación
pip install -r requirements.txt

## Ejecución
python -m uvicorn main:app --reload

## Endpoints disponibles
- GET /students
- GET /students/{id}

## Testing 
python -m pytest

## Docker
docker build -t daw-backend .
docker run -p 8000:8000 daw-backend

## CI/CD – GitHub Actions
Workflows ubicados en backend/.github/workflows/
- backend-test.yml
- backend-docker.yml

Requiere secrets:
- DOCKERHUB_USERNAME
- DOCKERHUB_TOKEN

## Añadimos la informacion impresa que resume los remotos
gitlab  https://gitlab.com/nereasancheztornel/gitlab.git (fetch)
gitlab  https://gitlab.com/nereasancheztornel/gitlab.git (push)
origin  https://github.com/NereaSanchez77/backend.git (fetch)
origin  https://github.com/NereaSanchez77/backend.git (push)
