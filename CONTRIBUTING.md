## **Cómo Contribuir al Repositorio**

Contribuir a este repositorio es sencillo si sigues los pasos a continuación. Esto te ayudará a mantener un flujo de trabajo organizado y colaborativo.

### **1. Hacer un Fork del Repositorio**

- Ve a la página principal del repositorio.
- Haz clic en el botón **"Fork"** en la esquina superior derecha para crear tu propia copia del repositorio.  
  [Más información sobre Forks.](https://docs.github.com/es/get-started/quickstart/fork-a-repo)

---

### **2. Clonar el Repositorio**

- Abre tu terminal o consola de comandos.
- Ejecuta el siguiente comando para clonar el repositorio en tu máquina local:

  ```bash
  git clone https://github.com/tu-usuario/tu-repositorio.git
  cd tu-repositorio
  ```

[¿Qué es clonar un repositorio?](https://docs.github.com/es/repositories/creating-and-managing-repositories/cloning-a-repository)

---

### **3. Crear una Nueva Rama**

- Antes de realizar cualquier cambio, crea una nueva rama para trabajar. Esto ayuda a mantener organizada la línea principal del proyecto:

  ```bash
  git checkout -b nombre-de-tu-rama
  ```

- Usa nombres de ramas descriptivos, como `feature-agregar-seccion` o `fix-error-ortografia`.

[¿Qué es una rama en Git?](https://git-scm.com/book/es/v2/Ramificaciones-en-Git-Ramificar-y-Mergear)

---

### **4. Realizar Cambios**

- Abre el proyecto en tu editor de código preferido (por ejemplo, VS Code).
- Realiza los cambios necesarios, asegurándote de seguir las buenas prácticas del proyecto.

> **Tips:**
>
> - Sigue la estructura del código existente.
> - Asegúrate de que los archivos editados estén bien documentados.
> - Prueba tus cambios antes de proceder.

---

### **5. Confirmar los Cambios**

- Una vez que completes tus cambios, guarda los archivos y confirma tus modificaciones. Usa comandos claros para registrar tus cambios:

  ```bash
  git add .
  git commit -m "Descripción clara del cambio realizado"
  ```

[¿Qué es un commit en Git?](https://git-scm.com/docs/git-commit)

---

### **6. Subir la Rama al Repositorio Remoto**

- Sube tu rama al repositorio remoto con el siguiente comando:

  ```bash
  git push origin nombre-de-tu-rama
  ```

[¿Qué es un push en Git?](https://git-scm.com/docs/git-push)

---

### **7. Crear un Pull Request**

- Ve a tu repositorio en GitHub.
- Haz clic en el botón **"Compare & pull request"** que aparecerá después de subir tu rama.
- Escribe una descripción detallada de los cambios que realizaste.
- Solicita la revisión de tus cambios y, si todo está en orden, el Pull Request será fusionado.

[¿Qué es un Pull Request?](https://docs.github.com/es/pull-requests)

---

### **8. Sincronizar el Repositorio Local**

- Una vez que tu contribución sea aceptada y fusionada, sincroniza tu repositorio local con el remoto para mantenerlo actualizado.
  ```bash
  git checkout main
  git pull upstream main
  ```

[¿Qué es sincronizar un repositorio?](https://www.atlassian.com/es/git/tutorials/syncing)

---

## **Reglas para Contribuir**

1. **Revisa las Issues:** Antes de comenzar, verifica si existe una _issue_ relacionada con tu cambio. Si no existe, crea una nueva.  
   [¿Qué son las Issues en GitHub?](https://docs.github.com/es/issues)
2. **Sigue las Convenciones:** Respeta las guías de estilo y estructura del proyecto.
3. **Documenta tus Cambios:** Asegúrate de incluir comentarios o actualizaciones en la documentación, si es necesario.
4. **Mantén tu Rama Limpiamente Actualizada:** Siempre sincroniza tu rama con `main` antes de hacer un Pull Request.
