# 🧠 GLOSARIO DE COMANDOS CMD Y GIT PARA CONTROL DE VERSIONES (Nivel Junior)

## 🖥️ CMD (Windows Command Prompt)

### 📁 Gestión de Archivos y Directorios

| Comando | Descripción | Ejemplo |
|----------|--------------|----------|
| `dir` | Muestra los archivos y carpetas del directorio actual. | `dir` |
| `cd` | Cambia de directorio (carpeta). | `cd proyecto` / `cd ..` |
| `mkdir` | Crea un nuevo directorio. | `mkdir nueva_carpeta` |
| `rmdir` | Elimina un directorio vacío. | `rmdir vieja_carpeta` |
| `del` | Elimina un archivo. ⚠️ | `del archivo.txt` |
| `copy` | Copia archivos de un lugar a otro. | `copy archivo.txt D:\backup` |
| `move` | Mueve o renombra archivos. | `move archivo.txt nueva_carpeta\` |
| `cls` | Limpia la pantalla de la terminal. | `cls` |
| `exit` | Cierra la ventana de CMD. | `exit` |
| `type` | Muestra el contenido de un archivo de texto. | `type README.md` |

---

## 🧰 GIT (Control de Versiones)

### 🔧 Configuración Inicial

| Comando | Descripción | Ejemplo |
|----------|--------------|----------|
| `git config --global user.name` | Define tu nombre de usuario. | `git config --global user.name "Josep"` |
| `git config --global user.email` | Define tu correo (para los commits). | `git config --global user.email "tucorreo@example.com"` |
| `git config --list` | Muestra la configuración actual. | `git config --list` |

---

### 🏁 Inicio y Clonación

| Comando | Descripción | Ejemplo |
|----------|--------------|----------|
| `git init` | Inicializa un nuevo repositorio en la carpeta actual. | `git init` |
| `git clone` | Clona (descarga) un repositorio existente. | `git clone https://github.com/usuario/repositorio.git` |

---

### 💾 Control de Cambios

| Comando | Descripción | Ejemplo |
|----------|--------------|----------|
| `git status` | Muestra el estado actual del repositorio. | `git status` |
| `git add` | Añade archivos al área de preparación (staging). | `git add archivo.js` o `git add .` |
| `git commit -m` | Guarda los cambios en el historial con un mensaje. | `git commit -m "Agrega nueva funcionalidad"` |
| `git log` | Muestra el historial de commits. | `git log` |
| `git diff` | Muestra diferencias entre versiones de archivos. | `git diff` |
| `git restore` | Restaura archivos modificados sin guardar. | `git restore archivo.js` |

---

### 🌿 Ramas (Branches)

| Comando | Descripción | Ejemplo |
|----------|--------------|----------|
| `git branch` | Lista todas las ramas. | `git branch` |
| `git branch nombre-rama` | Crea una nueva rama. | `git branch feature-login` |
| `git checkout nombre-rama` | Cambia a otra rama. | `git checkout feature-login` |
| `git switch nombre-rama` | Alternativa moderna a `checkout`. | `git switch main` |
| `git merge nombre-rama` | Fusiona una rama con la actual. | `git merge feature-login` |
| `git branch -d nombre-rama` | Elimina una rama local. | `git branch -d feature-login` |

---

### 🔄 Sincronización con Repositorio Remoto

| Comando | Descripción | Ejemplo |
|----------|--------------|----------|
| `git remote -v` | Muestra los remotos configurados. | `git remote -v` |
| `git remote add origin` | Vincula un repositorio remoto. | `git remote add origin https://github.com/usuario/repo.git` |
| `git push` | Envía tus commits al repositorio remoto. | `git push origin main` |
| `git pull` | Descarga y fusiona los cambios del remoto. | `git pull origin main` |
| `git fetch` | Descarga cambios del remoto **sin** fusionarlos. | `git fetch origin` |

---

### 🧹 Otros Comandos Útiles

| Comando | Descripción | Ejemplo |
|----------|--------------|----------|
| `git stash` | Guarda temporalmente cambios sin hacer commit. | `git stash` |
| `git stash pop` | Restaura los cambios guardados. | `git stash pop` |
| `git revert <commit>` | Revierte un commit anterior. | `git revert 3a5b6c7` |
| `git reset --hard <commit>` | Regresa el repo a un estado anterior (⚠️). | `git reset --hard HEAD~1` |
| `git tag` | Crea o lista etiquetas (versiones). | `git tag v1.0` |

---

## 💡 Consejos Clave para un Junior

- Usa `git status` **todo el tiempo**: te dice qué está pasando.  
- Haz commits **pequeños y frecuentes**, con mensajes claros.  
- Antes de hacer `git push`, asegúrate de haber hecho `git pull`.  
- Crea ramas para cada tarea o feature.  
- Si algo sale mal: `git log` + `git checkout` son tus mejores amigos.  
- Recuerda: **Git no es magia**, pero te salva la vida cuando aprendes a usarlo bien.

---

✨ **Autor:** Josep  
📁 **Propósito:** Referencia rápida de comandos CMD y Git para control de versiones.  
