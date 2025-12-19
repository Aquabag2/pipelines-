# Guía Paso a Paso: Cómo Usar el Pipeline 🚀

## ⚠️ IMPORTANTE: Los pipelines NO se activan con comandos locales
Se ejecutan **automáticamente** cuando subes tu código a GitLab o GitHub.

---

## Opción 1: Usar con GitLab (Más fácil) 🦊

### Paso 1: Crear repositorio en GitLab
1. Ve a https://gitlab.com
2. Inicia sesión o créate una cuenta
3. Haz clic en "New project" → "Create blank project"
4. Ponle un nombre: **"pipeline"**
5. NO marques "Initialize repository with a README"
6. Copia la URL que te da (ej: `https://gitlab.com/tu-usuario/pipeline.git`)

### Paso 2: Subir tu código
Abre tu terminal en la carpeta del proyecto y escribe:

```bash
git init
git add .
git commit -m "Primer commit con pipeline"
git remote add origin https://gitlab.com/tu-usuario/pipeline.git
git push -u origin main
```

### Paso 3: ¡Ver el pipeline en acción!
1. Ve a tu proyecto en GitLab
2. En el menú lateral, haz clic en **"CI/CD"** → **"Pipelines"**
3. ¡Ahí verás tu pipeline ejecutándose!

---

## Opción 2: Usar con GitHub 🐙

### Paso 1: Crear repositorio en GitHub
1. Ve a https://github.com
2. Inicia sesión o créate una cuenta
3. Haz clic en el "+" arriba a la derecha → "New repository"
4. Ponle un nombre: **"pipeline"**
5. NO marques "Add a README file"
6. Haz clic en "Create repository"
7. Copia la URL que te da (ej: `https://github.com/tu-usuario/pipeline.git`)

### Paso 2: Subir tu código
Abre tu terminal en la carpeta del proyecto y escribe:

```bash
git init
git add .
git commit -m "Primer commit con pipeline"
git remote add origin https://github.com/tu-usuario/pipeline.git
git push -u origin main
```

### Paso 3: ¡Ver el pipeline en acción!
1. Ve a tu proyecto en GitHub
2. Haz clic en la pestaña **"Actions"** (arriba del repositorio)
3. ¡Ahí verás tu pipeline ejecutándose!

---

## 🔍 ¿Qué verás cuando funcione?

### En GitLab:
```
Pipelines
├── #123 (running) ← Pipeline ejecutándose
    ├── test: running ✅
    └── build: pending ⏳
```

### En GitHub:
```
Actions
├── CI Pipeline (#1) - running
    ├── test: running ✅
    └── build: pending ⏳
```

---

## ❓ Preguntas Frecuentes

### ¿Necesito instalar algo?
**NO**. Todo funciona en la nube (GitLab/GitHub).

### ¿Funciona si no tengo tests o requirements.txt?
**SÍ**. El pipeline está hecho para que funcione aunque no tengas esos archivos.

### ¿Se ejecuta cada vez que hago push?
**SÍ**. Cada vez que subas código (push), el pipeline se ejecuta automáticamente.

### ¿Puedo probarlo localmente sin subirlo?
Sí, pero es más complicado. Solo para curiosos:
- GitLab: Necesitas instalar `gitlab-runner`
- GitHub: Necesitas instalar `act`

Pero **NO es necesario**. Es más fácil subirlo a GitLab/GitHub.

---

## 📝 Resumen Ultra Simple:

1. Crea cuenta en GitLab o GitHub
2. Crea un repositorio nuevo llamado **"pipeline"**
3. Ejecuta estos comandos (cambia "tu-usuario" por tu usuario):
   ```bash
   git init
   git add .
   git commit -m "Primer commit"
   git remote add origin https://gitlab.com/tu-usuario/pipeline.git
   # O para GitHub: git remote add origin https://github.com/tu-usuario/pipeline.git
   git push -u origin main
   ```
4. Ve a CI/CD (GitLab) o Actions (GitHub)
5. ¡Listo! Ya está funcionando 🎉

