# Documentación - Sesión 1

## Tema: Convención de Nombres de Ramas (HU) y Commits

En esta sesión se trabajó en la comprensión y aplicación de una convención estandarizada para la creación de ramas y mensajes de commit en el repositorio, con el fin de mantener orden, trazabilidad y coherencia entre los desarrolladores.

---

## 1. Estructura de la Rama

**Formato general:**

### Componentes:
- **tipo-trabajo:**  
  - `feature`: nueva funcionalidad.  
  - `bugfix`: corrección de defectos.  
  - `hotfix`: corrección urgente en producción.  
  - `refactor`: cambios internos sin alterar el comportamiento.  
  - `chore`: tareas de mantenimiento.  
  - `spike`: investigación o experimento.

- **stack:**  
  - `app-movil`: código de la aplicación móvil.  
  - `backend`: servicios o APIs del lado del servidor.  
  - `data-base`: esquemas, funciones, vistas, migraciones de base de datos.  
  - `doc`: documentación.

- **HU-<id>:** Identificador de la historia de usuario (1–6 dígitos).

- **ambiente:**  
  - `dev`: desarrollo.  
  - `qa`: pruebas.  
  - `main`: rama estable principal.  
  - `project`: integración temporal de un proyecto.

- **breve-descripcion (opcional):**  
  - 3–6 palabras en *kebab-case*.  
  - Sin acentos ni “ñ” (usar “n”).

---

## 2. Ejemplos de Ramas

Para garantizar consistencia, se definieron ejemplos claros de cómo deben nombrarse las ramas según la convención establecida.

### Ejemplos **sin** descripción opcional:
Estos casos se usan cuando la rama está directamente ligada a la HU y no es necesario agregar detalles adicionales en el nombre.



📌 **Nota:**  
- La descripción debe ir siempre en minúsculas.  
- El guion `-` se usa para separar palabras.  
- Evitar artículos y palabras innecesarias para mantenerlo corto y específico.  


---

## 3. Convención para Commits (Conventional Commits en inglés)

Durante la sesión, se revisó el uso de **Conventional Commits**, un estándar que define cómo redactar mensajes claros y consistentes en cada commit.

**Formato general del mensaje:**
feat(app-mobile): add offline cache for invoices (HU-19630)
fix(backend): handle null payer id in GET /billing/taxpayers (HU-19752)
refactor(database): split large procedure into smaller units (HU-21007)
chore(docs): update branching convention
