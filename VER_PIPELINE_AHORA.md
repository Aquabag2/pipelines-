# Cómo Ver tu Pipeline Ahora 🚀

## Pasos para ver el pipeline en GitHub:

### 1. Abre tu repositorio
👉 **https://github.com/Aquabag2/pipelines-**

### 2. Haz clic en "Actions"
En la parte superior del repositorio, verás estas pestañas:
```
Code | Issues | Pull requests | Actions | Projects | ...
                      ↑
                   Haz clic aquí
```

### 3. Primera vez - Activar GitHub Actions
Si es la primera vez que abres Actions, GitHub te mostrará:
- Un mensaje como "Get started with GitHub Actions"
- O "No workflow runs found yet"
- Haz clic en "I understand my workflows, go ahead and enable them" o similar

### 4. Si no aparece ningún pipeline ejecutado:
Necesitas hacer un nuevo push para activarlo. Ve a tu terminal y ejecuta:
```bash
git add .
git commit -m "Activar pipeline"
git push
```

### 5. Después del push, verás:
```
CI Pipeline (#1) - running (o completed)
    ├── test ✅
    └── build ✅
```

**NOTA:** El pipeline se ejecuta AUTOMÁTICAMENTE cada vez que haces push a la rama main.

### 4. Haz clic en el pipeline para ver los detalles
- Verás los logs de cada paso
- Puedes ver qué comandos se ejecutaron
- Verás si pasó o falló cada paso

---

## ¿Qué deberías ver?

Si todo funciona bien:
- ✅ **test**: Instalando dependencias... → Tests completados!
- ✅ **build**: Construyendo proyecto... → Build completado!

Si hay algún problema:
- ❌ Verás en rojo qué falló
- Puedes hacer clic para ver los logs del error

---

## 📸 ¿Dónde está exactamente?

```
GitHub.com
└── Aquabag2
    └── pipelines- (tu repositorio)
        └── [Pestaña "Actions"] ← AQUÍ
            └── CI Pipeline
                ├── test
                └── build
```

---

## 🔄 Si no aparece el pipeline:

1. Espera unos segundos (puede tardar en aparecer)
2. Refresca la página (F5 o Cmd+R)
3. Asegúrate de estar en la pestaña "Actions"
4. Busca "CI Pipeline" en la lista

¡Ya deberías poder verlo funcionando! 🎉

