# 🎓 Curso Práctico de GitHub: De Cero a Maestro

Bienvenido a tu repositorio de aprendizaje. Este documento es interactivo: lee las instrucciones y realiza las acciones directamente en la plataforma.

---

## 📊 Mi Progreso de Aprendizaje

_Marca cada función a medida que la domines:_

- [ ] 1. Conceptos y Configuración
- [ ] 2. El Repositorio
- [ ] 3. Subir el código (Add, Commit, Push)
- [ ] 4. Bajar el código (Clone)
- [ ] 5. Sincronizar cambios (Pull)
- [ ] 6. Privacidad y Seguridad
- [ ] 7. El archivo .gitignore
- [ ] 8. Seguimiento y Gestión (Issues/Projects)

---

## 🛠️ Módulos de Aprendizaje

Haz clic en cada sección para desplegar la lección y la práctica:

---

### 1️⃣ Conceptos y Configuración

Antes de empezar, es fundamental diferenciar entre **Git** y **GitHub**.

**Git** es el programa que registra los cambios en tus archivos (el motor del historial). Sin él, no puedes hacer nada de lo que aprenderás aquí.

**GitHub** es la plataforma en la nube donde guardas esos archivos y colaboras con otros. Es como "Google Drive pero para código".

**¿Ya tienes instalado Git?**

- [📥 Descargar Git](https://git-scm.com/download/win)
- [📥 Descargar GitHub Desktop](https://desktop.github.com/) (más fácil para principiantes)

**Acción:** Abre GitHub Desktop después de instalar. Te pedirá que inicies sesión con tu cuenta de GitHub.

---

### 2️⃣ El Repositorio

El "repositorio" es la carpeta de tu proyecto, pero alojada en la nube.

**¿Estás viendo un repositorio ahora mismo?** Observa el nombre arriba a la izquierda de esta página:

<img width="280" alt="Captura de nombre de repositorio" src="https://github.com/user-attachments/assets/180e053a-eaf0-4ec7-b2c9-f13e6fd5fb99" />

GitHub además de ser la nube para tus desarrollos, funciona como una **red social** donde puedes encontrar otros programadores y recursos. Míralo como una **Enciclopedia de Soluciones**.

**Acción práctica:** Intenta crear un repositorio nuevo desde el botón `+` en la barra superior de GitHub.

<img width="130" alt="Botón crear nuevo" src="https://github.com/user-attachments/assets/5a3110b5-ccf9-420e-ab7f-327d726c08a0" />

---

### 3️⃣ Subir el código (Add, Commit, Push)

Este es el **"Ciclo de Guardado"** profesional. Cada vez que termines una tarea importante, harás estos tres pasos:

**1. Add:** Eliges qué archivos quieres guardar.

```bash
git add .
```

> El punto `.` significa "todos los archivos". También puedes especificar uno por uno:
>
> ```bash
> git add index.html
> git add styles.css
> ```

**2. Commit:** Tomas una "foto" del estado actual con una descripción.

```bash
git commit -m "Mi primer commit: Agregué el formulario de contacto"
```

> **Consejo:** El mensaje debe ser claro y corto. Imagina que le dices a alguien qué hiciste en una frase.

**3. Push:** Subes esa foto a la nube.

```bash
git push origin main
```

---

**Analogía del correo 📦:**

| Paso     | Analogía                  | Descripción                  |
| -------- | ------------------------- | ---------------------------- |
| `add`    | Empacar 📦                | Seleccionas qué vas a enviar |
| `commit` | Escribir la dirección 📝  | Le pones un标签 al paquete   |
| `push`   | Depositar en el correo 🚚 | Lo envías a la nube          |

---

**Acción práctica:**

1. Haz un cambio en cualquier archivo de este repositorio (por ejemplo, edita este markdown)
2. Abre GitHub Desktop
3. Verás los cambios en la columna izquierda
4. Escribe un mensaje de commit
5. Presiona **Commit to main**
6. Presiona **Push Origin**

---

### 4️⃣ Bajar el código (Clone)

¿Tienes un repositorio en la nube y quieres una copia exacta en tu computadora? Eso es **clonar**.

**Acción práctica:**

1. Ve al repositorio que quieras bajar
2. Haz clic en el botón verde **"<> Code"** que está arriba de este archivo
3. Selecciona **"Open with GitHub Desktop"**
4. Elige dónde guardarlo en tu computadora

¡Listo! Ahora tienes una copia exacta en tu PC.

---

### 5️⃣ Sincronizar cambios (Pull)

Imagina que trabajaste en tu código desde tu PC. Luego alguien más hizo cambios en la misma nube.

¿Qué pasa si ambos editaron el mismo archivo? ¡Conflicto! Por eso existe **Pull**.

**Pull** significa: "Baja los cambios de la nube y fusiónalos con mi código local".

**Acción práctica:**

1. Haz un cambio en la web (edita cualquier archivo aquí mismo)
2. Abre GitHub Desktop
3. Presiona **Pull Origin**
4. Verás cómo se actualiza tu código local

---

### 6️⃣ Privacidad y Seguridad

Aprende a decidir quién ve tu trabajo.

**Hay dos tipos de repositorios:**

| Tipo           | Visibilidad | ¿Quién lo ve?                         |
| -------------- | ----------- | ------------------------------------- |
| **Público** 🌐 | Abierto     | Cualquier persona en internet         |
| **Privado** 🔒 | Cerrado     | Solo tú y las personas que tú invites |

**Acción práctica:**

1. Ve a la pestaña de **Settings** de este repositorio
2. Busca la sección **"Change visibility"**
3. Experimenta cambiando de público a privado y viceversa

[⚙️ Ir a Ajustes](../../settings)

**¿Cuándo usar cada uno?**

- **Público:** Para proyectos open source, tu portafolio, o cuando quieres que otros aprendan de tu código
- **Privado:** Para proyectos de trabajo, código con información sensible, o mientras estás desarrollando

---

### 7️⃣ El archivo .gitignore (¡Muy importante!)

Antes de subir tu código, crea un archivo llamado `.gitignore` en la raíz de tu proyecto.

Este archivo le dice a Git **qué archivos NO subir** a la nube.

**¿Por qué es importante?**

Imagina que subiste una carpeta `fotos/` de 500 MB. Tardaría horas y consume espacio innecesario.

O peor: subiste un archivo `.env` que contiene tu contraseña de base de datos. ¡Cualquiera podría verla!

**Ejemplo de .gitignore típico:**

```
# Carpetas que no нужно subir
node_modules/
.env
vendor/

# Archivos temporales
*.log
*.tmp

# Fotos y documentos grandes
*.png
*.jpg
*.pdf
```

**Acción práctica:**

1. Crea un nuevo archivo llamado `.gitignore` en la raíz de tu proyecto
2. Agrega las líneas según tu proyecto
3. Haz commit y push

---

### 8️⃣ Seguimiento (Issues y Proyectos)

GitHub no es solo código, también sirve para organizar trabajo.

**Issues (Tareas):** Úsalos para reportar errores o planear tareas.

Ejemplo: "El botón de login no funciona" o "Agregar modo oscuro"

**Proyectos (Tableros):** Tableros visuales tipo Kanban para organizar el flujo de trabajo.

Es como un tablero de Trello integrado con tu código.

**Acción práctica:**

1. Crea un Issue nuevo
2. Asígnale etiquetas (bugs, features, preguntas)
3. O crea un Proyecto y agrega tus Issues como tarjetas

[📝 Ver mis Tareas (Issues)](../../issues) | [📋 Ver el Tablero (Projects)](../../projects)

---

## 💡 Tips para Alumnos

**Tip 1 - Editor rápido:**
Para editar cualquier archivo de este curso rápidamente, presiona la tecla `.` (punto) en tu teclado mientras estás en esta página. ¡Se abrirá un editor de código (VS Code web) directamente en tu navegador!

**Tip 2 - Atajos útiles:**

| Atajo | Qué hace                    |
| ----- | --------------------------- |
| `t`   | Buscar archivos rápidamente |
| `l`   | Ir a una línea específica   |
| `w`   | Cambiar vista (wide/narrow) |
| `/`   | Buscar en el repositorio    |

**Tip 3 - Commits pequeños:**
Es mejor hacer muchos commits pequeños que uno grande. Cada commit debe representar UNA tarea completada.

---

## 🎯 Resumen Rápido

| Comando               | Qué hace            | Analogía      |
| --------------------- | ------------------- | ------------- |
| `git add .`           | Selecciona archivos | Empacar 📦    |
| `git commit -m "..."` | Guardar con mensaje | Etiquetar 📝  |
| `git push`            | Subir a la nube     | Enviar 🚚     |
| `git clone`           | Bajar repositorio   | Descargar 📥  |
| `git pull`            | Traer cambios       | Actualizar 🔄 |

---

## ✅ Tu Checklist Final

Antes de subir tu código, verifica:

- [ ] ¿Creé un archivo `.gitignore`?
- [ ] ¿Incluí todos los archivos importantes?
- [ ] ¿Excluí carpetas innecesarias (node_modules, .env)?
- [ ] ¿Escribí un mensaje de commit claro?
- [ ] ¿Revisé dos veces antes de hacer Push?

---

¡Felicitaciones por completar el curso! Ahora ya sabes lo básico para trabajar con Git y GitHub.

**Próximos pasos sugeridos:**

- Aprende a crear ramas (branches) para trabajar en paralelo
- Practica resolver conflictos de código
- Explora repositorios públicos para aprender de otros
