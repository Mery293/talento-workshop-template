# **Documentación del Archivo de Configuración (CONFIG.json)**

El archivo `CONFIG.json` contiene la configuración necesaria para personalizar tu página personal. A continuación, se explica cada propiedad del archivo, cómo agregar o quitar información, y cómo realizar el despliegue en Vercel después de actualizarlo.

---

## **Estructura del Archivo**

### **1. `personalInfo`**

Esta sección contiene información personal del usuario.

#### Propiedades:

- **`firstName` (string):** Primer nombre del usuario.
  - Ejemplo: "Brayan".
- **`lastName` (string):** Apellido del usuario.
  - Ejemplo: "Montaño".
- **`about` (string):** Breve descripción sobre el usuario.
  - Ejemplo: "Soy un desarrollador de software especializado en javascript y react."
- **`birthDate` (string):** Fecha de nacimiento en formato `AAAA-MM-DD`.
  - Ejemplo: "1999-08-29".
- **`email` (string):** Dirección de correo electrónico.
  - Ejemplo: "brayanmbeltre@gmail.com".
- **`github` (string):** URL al perfil de GitHub.
  - Ejemplo: "https://github.com/brayanMBeltre".
- **`linkedin` (string):** URL al perfil de LinkedIn.
  - Ejemplo: "https://www.linkedin.com/in/brayanmbeltre/".

---

### **2. `skills`**

Lista de habilidades del usuario.

#### Formato:

Un array de strings, donde cada string representa una habilidad.

- Ejemplo:
  ```json
  "skills": [
    "Javascript",
    "React",
    "GraphQL"
  ]
  ```

#### Para agregar o quitar habilidades:

- **Agregar:** Incluye una nueva habilidad al array:
  ```json
  "skills": [
    "Javascript",
    "React",
    "GraphQL",
    "Node.js"
  ]
  ```
- **Quitar:** Elimina la habilidad que ya no desees listar.

---

### **3. `experiences`**

Lista de experiencias laborales del usuario.

#### Formato:

Un array de objetos, donde cada objeto contiene:

- **`dates` (string):** Período de trabajo.
  - Ejemplo: "2021".
- **`role` (string):** Puesto desempeñado.
  - Ejemplo: "Frontend Developer".
- **`company` (string):** Nombre de la empresa.
  - Ejemplo: "OGTIC".
- **`description` (string):** Descripción breve del trabajo realizado.
  - Ejemplo: "Trabajé en proyectos como Becas.gob.do, Gob.do, 311, entre otros, realizando tareas de desarrollo frontend."
- **`logo` (string):** URL del logotipo de la empresa.
  - Ejemplo: "https://ogtic.gob.do/logo.png".

#### Para agregar una experiencia:

1. Crea un nuevo objeto con el mismo formato:
   ```json
   {
     "dates": "2022",
     "role": "Backend Developer",
     "company": "Tech Corp",
     "description": "Desarrollo de APIs RESTful utilizando Node.js.",
     "logo": "https://techcorp.com/logo.png"
   }
   ```
2. Añádelo al array `experiences`.

#### Para eliminar una experiencia:

- Borra el objeto correspondiente dentro del array.

---

### **4. `projects`**

Lista de proyectos destacados realizados por el usuario.

#### Formato:

Un array de objetos, donde cada objeto contiene:

- **`name` (string):** Nombre del proyecto.
  - Ejemplo: "Dynamic portfolio creation".
- **`description` (string):** Breve descripción del proyecto.
  - Ejemplo: "Crear un portafolio genérico a partir de un JSON para estudiantes del proyecto 'Semillero Digital' impartido en la OGTIC."
- **`image` (string):** URL de la imagen representativa del proyecto.
  - Ejemplo: "https://ogtic.gob.do/_next/image?url=https%3A%2F%2Fwp.ogtic.gob.do%2Fwp-content%2Fuploads%2F2024%2F01%2Flogo.png&w=3840&q=75".
- **`url` (string):** Enlace al proyecto (puede ser un repositorio o una página desplegada).
  - Ejemplo: "https://github.com/BrayanMBeltre/talento-workshop-template".

#### Para agregar un proyecto:

1. Crea un nuevo objeto con el mismo formato:
   ```json
   {
     "name": "Nueva aplicación",
     "description": "Aplicación de gestión de tareas desarrollada en React.",
     "image": "https://miapp.com/imagen.png",
     "url": "https://github.com/miusuario/nueva-aplicacion"
   }
   ```
2. Añádelo al array `projects`.

#### Para eliminar un proyecto:

- Borra el objeto correspondiente dentro del array.

---

## **Cómo Subir los Cambios y Redesplegar en Vercel**

### **1. Realizar Cambios en `CONFIG.json`**

1. Abre el archivo `CONFIG.json` en tu editor de texto o código.
2. Realiza los cambios necesarios siguiendo la estructura descrita anteriormente.
3. Guarda el archivo.

### **2. Confirmar y Subir Cambios a GitHub**

1. Abre tu terminal y navega al repositorio local.
2. Asegúrate de estar en la rama correcta (por ejemplo, `main`).
3. Ejecuta los siguientes comandos:
   ```bash
   git add CONFIG.json
   git commit -m "Actualización del archivo de configuración."
   git push origin main
   ```

### **3. Verificar el Redespliegue en Vercel**

1. Una vez que los cambios se suban a GitHub, Vercel iniciará el despliegue automático.
2. Ve a tu dashboard en [Vercel](https://vercel.com/) para verificar el estado del despliegue.
3. Cuando el despliegue finalice, revisa tu sitio para confirmar que los cambios se aplicaron correctamente.

---

Si tienes dudas adicionales, consulta la documentación oficial de:

- [JSON](https://www.json.org/json-es.html)
- [Git](https://git-scm.com/doc)
- [Vercel](https://vercel.com/docs)
