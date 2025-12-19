# Pipeline Simple

Este es un ejemplo simple de pipeline CI/CD.

## GitLab CI

El archivo `.gitlab-ci.yml` define el pipeline para GitLab.

### Qué hace:
1. **test**: Ejecuta los tests del proyecto
2. **build**: Construye el proyecto (solo en main/master)

## GitHub Actions

El archivo `.github/workflows/ci.yml` define el pipeline para GitHub.

### Qué hace:
1. **test**: Instala dependencias y ejecuta tests
2. **build**: Construye el proyecto después de que pasen los tests

## Cómo usarlo:

### Para GitLab:
- Sube el archivo `.gitlab-ci.yml` a la raíz de tu repositorio
- GitLab automáticamente detectará y ejecutará el pipeline

### Para GitHub:
- Sube la carpeta `.github/workflows/` con el archivo `ci.yml`
- GitHub automáticamente detectará y ejecutará el workflow

