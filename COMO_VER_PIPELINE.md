# Cómo Ver el Pipeline 👀

## 1. Ver los archivos localmente

Ya puedes ver los archivos en tu editor. Los archivos son:

- `.gitlab-ci.yml` - Pipeline para GitLab
- `.github/workflows/ci.yml` - Pipeline para GitHub

## 2. Verlo en GitLab 🦊

### Pasos:
1. **Sube tu código a GitLab:**
   ```bash
   git init
   git add .
   git commit -m "Añadir pipeline CI"
   git remote add origin https://gitlab.com/tu-usuario/tu-repo.git
   git push -u origin main
   ```

2. **En GitLab, ve a:**
   - **CI/CD** → **Pipelines** (en el menú lateral)
   - O ve directamente a: `https://gitlab.com/tu-usuario/tu-repo/-/pipelines`

3. **Verás:**
   - Lista de todos los pipelines ejecutados
   - Estado de cada pipeline (passed/failed/running)
   - Puedes hacer clic en uno para ver los jobs individuales (test, build)

## 3. Verlo en GitHub 🐙

### Pasos:
1. **Sube tu código a GitHub:**
   ```bash
   git init
   git add .
   git commit -m "Añadir pipeline CI"
   git remote add origin https://github.com/tu-usuario/tu-repo.git
   git push -u origin main
   ```

2. **En GitHub, ve a:**
   - **Actions** (pestaña superior del repositorio)
   - O directamente: `https://github.com/tu-usuario/tu-repo/actions`

3. **Verás:**
   - Lista de todos los workflows ejecutados
   - Estado de cada ejecución (verde ✅ = éxito, rojo ❌ = fallo)
   - Haz clic en uno para ver los jobs (test, build) y los logs

## 4. Probar localmente (opcional) 🔧

### Para GitLab CI:
```bash
# Necesitas GitLab Runner instalado
gitlab-runner exec docker test
gitlab-runner exec docker build
```

### Para GitHub Actions:
```bash
# Necesitas act instalado (https://github.com/nektos/act)
act -l  # Lista los workflows
act     # Ejecuta el workflow
```

## Resumen rápido:

- **Localmente:** Ya lo estás viendo en tu editor 📝
- **GitLab:** CI/CD → Pipelines 🦊
- **GitHub:** Pestaña Actions 🐙

¡Simplemente sube el código y los pipelines se ejecutarán automáticamente en cada push!

