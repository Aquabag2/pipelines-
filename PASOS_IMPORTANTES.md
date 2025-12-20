# ⚠️ PASOS IMPORTANTES - No te los saltes!

## Antes de hacer `git push`, DEBES:

### 1. Crear el repositorio en GitHub primero:

1. Ve a: **https://github.com/new**
2. Nombre del repositorio: **pipeline**
3. ⚠️ **NO marques** "Add a README file"
4. Haz clic en **"Create repository"**

### 2. Después ejecuta estos comandos:

```bash
git init
git add .
git commit -m "Primer commit con pipeline"
git remote add origin https://github.com/Aquabag2/pipeline.git
git push -u origin main
```

---

## Si ya ejecutaste `git init` y `git add`:

Solo necesitas hacer commit y push:

```bash
git commit -m "Primer commit con pipeline"
git push -u origin main
```

---

## Resumen rápido:

✅ **PRIMERO**: Crea el repositorio en GitHub (https://github.com/new)  
✅ **DESPUÉS**: Ejecuta los comandos git

Si intentas hacer push antes de crear el repositorio, te dará error: "repository not found"

