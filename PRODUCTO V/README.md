# PRODUCTO V: Gestión de Configuración, Versionamiento y DevOps
### Universidad Nacional Experimental de Guayana (UNEG)
**Asignatura:** Ingeniería de Software II  
**Profesor:** Mg. Félix Márquez  
**Fecha de Entrega:** 22/09/2026  
**Equipo:** *Ingenio y Código*  

---

## 👥 Equipo de Trabajo
* **Rhixeidys Aguilera** — V-30.851.503
* **Yonkeiner Bravo** — V-30.994.057
* **Brayan Carreño** — V-32.015.527
* **Nicole García** — V-30.809.865

---

## 🔗 Enlaces de Evaluación Oficial

### 1. Repositorio Oficial del Proyecto de la Unidad V
Tal como lo solicitó el profesor Félix Márquez en las pautas oficiales de la evaluación:
> *«...colocar Producto V donde allí colocar la dirección del repositorio del proyecto en el cual realizaron su evaluación...»*

El equipo consolidó toda la arquitectura técnica, código fuente y flujos de integración en el siguiente repositorio oficial del proyecto:

👉 **[https://github.com/Bryd3n/ISII-Everything-as-Code-Demo](https://github.com/Bryd3n/ISII-Everything-as-Code-Demo)**

#### Evidencias prácticas implementadas en el repositorio:
1. **Flujo GitHub Flow & Pull Request (Pregunta 1):**
   * Rama de funcionalidad activa: `feature/pdf-export`.
   * **Pull Request #1 en vivo:** [https://github.com/Bryd3n/ISII-Everything-as-Code-Demo/pull/1](https://github.com/Bryd3n/ISII-Everything-as-Code-Demo/pull/1) con su plantilla estructurada de descripción, impacto y checklist de revisión.
2. **Everything as Code & Contenedorización Inmutable (Ejercicio 2):**
   * Microservicio Node.js en puerto 8080 con verificación en `/health`.
   * `Dockerfile` optimizado y comentado que erradica la deriva de configuración (*Configuration Drift*).
3. **Pipeline de Integración Continua (CI & Quality Gates):**
   * Automatización en GitHub Actions validando los 3 Quality Gates (tests unitarios, auditoría de seguridad `npm audit` y build de Docker).
4. **Orquestación Declarativa (Pregunta 4):**
   * Manifiestos versionados `.gitignore`, `Dockerfile`, `.github/workflows/ci.yml` y `docker-compose.yml`.

---

### 2. Video de la Defensa Oral (Google Drive)
* **Enlace de Google Drive:** *(Pendiente de enlazar tras la compilación final del video del equipo)*

---

## 📂 Archivos del Entregable
* `Ejercicio_2_y_Pregunta_4_Brayan.pdf`: Documento formal UNEG con portada institucional, resolución teórica de Dockerización, Deriva de Configuración y Artefactos de SCM.
* `01_Lamina_Defensa_Ejercicio_2_y_Pregunta_4_Brayan.png`: Lámina en formato 16:9 con espacio superior libre para cámara web en OBS y badge del repositorio oficial.
