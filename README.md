# Coberturas Fontanería — PWA

App instalable para consultar coberturas de fontanería. Funciona en Android, iOS y PC, con soporte offline.

---

## 🚀 Pasos para publicar en GitHub Pages

### 1. Crear el repositorio en GitHub
1. Entra en [github.com](https://github.com) → botón **"New"**
2. Nombre del repositorio: `coberturas-fontaneria` (o el que prefieras)
3. Visibilidad: **Public** ✅
4. **No** marques ninguna opción adicional (sin README, sin .gitignore)
5. Clic en **"Create repository"**

### 2. Subir los archivos
**Opción fácil — desde el navegador:**
1. En el repositorio vacío, clic en **"uploading an existing file"**
2. Arrastra todos los archivos y carpetas de este ZIP (manteniendo la estructura)
3. En el mensaje de commit escribe `Primera versión` y clic **"Commit changes"**

**Opción Git (terminal):**
```bash
cd carpeta-del-zip
git init
git add .
git commit -m "Primera versión"
git branch -M main
git remote add origin https://github.com/TU_USUARIO/coberturas-fontaneria.git
git push -u origin main
```

### 3. Activar GitHub Pages
1. En tu repositorio → **Settings** → **Pages** (menú izquierdo)
2. En **"Source"** selecciona **"GitHub Actions"**
3. Guarda. El workflow se ejecuta automáticamente.
4. En ~1 minuto la URL estará activa:
   `https://TU_USUARIO.github.io/coberturas-fontaneria/`

---

## 📱 Instalar la app

| Plataforma | Pasos |
|---|---|
| **Android** (Chrome) | Abre la URL → menú ⋮ → "Añadir a pantalla de inicio" |
| **iOS** (Safari) | Abre la URL → botón compartir □↑ → "Añadir a pantalla de inicio" |
| **PC** (Chrome/Edge) | Abre la URL → icono ⊕ en la barra de direcciones → "Instalar" |

> La app funciona **sin conexión** después de la primera carga.

---

## 📁 Estructura de archivos

```
/
├── index.html                    ← App principal
├── manifest.json                 ← Config PWA (nombre, iconos, colores)
├── sw.js                         ← Service Worker (offline)
├── favicon.ico
├── icons/
│   ├── icon-72.png  … icon-512.png
│   ├── icon-maskable-512.png     ← Para Android (fondo adaptable)
│   └── apple-touch-icon.png      ← Para iOS
└── .github/
    └── workflows/
        └── deploy.yml            ← Despliegue automático
```
