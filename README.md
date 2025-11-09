# Gimnasio Virtual - FitTech Solutions

Este repositorio contiene una versión estática (HTML/CSS) del gimnasio virtual solicitado. Incluye:

- `index.html` — página principal con el análisis biomecánico, plantillas de vídeo y análisis.
- `styles.css` — estilos básicos.
- `logo.svg` — placeholder del logo.

Instrucciones para crear el repositorio en GitHub, subirlo y desplegar en Netlify (resumen):

1. Inicializar git localmente (PowerShell):

```powershell
cd "c:\Users\jc430\Documents\Gimnasio"
git init
git add .
git commit -m "Initial: Gimnasio Virtual site"
```

2. Crear el repositorio en GitHub:

- Opción A (recomendada): crear el repo en https://github.com/new , copiar la URL remota y luego:

```powershell
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git
git branch -M main
git push -u origin main
```

- Opción B: si tienes GitHub CLI configurado:

```powershell
gh repo create REPO_NAME --public --source=. --remote=origin --push
```

3. Desplegar en Netlify:

- Accede a https://app.netlify.com/ y conecta tu cuenta.
- Selecciona "New site from Git" → GitHub → autoriza y elige el repositorio creado.
- Configure build settings: No build command (leave blank) and Publish directory: `/` (root) or `/` depending on Netlify. (Para un sitio estático simple no se necesita build).

4. Opcional: subir vídeos (mp4) a la rama `main` en carpeta `/videos` o alojarlos externamente (Google Drive, YouTube, etc.) y pegar enlaces en `index.html` o en el documento final.

Si quieres, puedo intentar inicializar git aquí y crear el primer commit localmente; pero no puedo crear el repositorio remoto en GitHub sin que autorices desde tu máquina (web o `gh`), por razones de autenticación. Te dejo los comandos anteriores listos para ejecutar en PowerShell.
