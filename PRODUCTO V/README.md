# PRODUCTO V: Gestión de Configuración, Versionamiento y DevOps
### Universidad Nacional Experimental de Guayana (UNEG)
**Vicerrectorado Académico | Coordinación de Ingeniería en Informática**  
**Asignatura:** Ingeniería de Software II – 7mo Semestre  
**Profesor:** Mg. Félix Márquez  
**Fecha de Entrega:** 22/09/2026  
**Equipo:** *Ingenio y Código*  

---

## 👥 Equipo de Trabajo y Distribución de Responsabilidades

| Integrante | Cédula | Rol / Asignación | Estado |
| :--- | :---: | :--- | :---: |
| **Rhixeidys Aguilera** | V-30.851.503 | **Ejercicio 1 (Pregunta 1):** Flujo Git ante incidentes (Stash, Hotfix, Rebase), Plantilla de PR y Quality Gates de CI | ✅ Listo (Lámina + Guión) |
| **Yonkeiner Bravo** | V-30.994.057 | **Pregunta 2:** GitFlow vs. Trunk-Based Development, Métricas DORA (*Accelerate*), Feature Flags y CD Avanzado | ✅ Listo (Lámina + Guión) |
| **Brayan Carreño** | V-32.015.527 | **Ejercicio 2 y Pregunta 4:** Everything as Code, Contenedorización Inmutable (Docker), Deriva de Configuración, CI/CD y Repositorio en Vivo | ✅ Listo (Informe + Repo + Lámina + Guión) |
| **Nicole García** | V-30.809.865 | **Pregunta 3:** Control de Cambios en Contextos Tradicionales (CCB) vs. Modernos (PRs y CI) | ⏳ En consolidación |

---

## 🔗 Enlaces de Evaluación Oficial

### 1. Repositorio Oficial del Proyecto de la Unidad V
Tal como lo solicitó el profesor Félix Márquez en las instrucciones oficiales:
> *«...colocar Producto V donde allí colocar la dirección del repositorio del proyecto en el cual realizaron su evaluación...»*

El equipo consolidó toda la arquitectura técnica, código fuente, pruebas automatizadas, manifiestos de infraestructura y pipelines en el siguiente repositorio oficial:

👉 **[https://github.com/Bryd3n/ISII-Everything-as-Code-Demo](https://github.com/Bryd3n/ISII-Everything-as-Code-Demo)**

#### Evidencias prácticas implementadas en el repositorio:
1. **Flujo GitHub Flow & Pull Request (Ejercicio 1 / Rhixeidys Aguilera):**
   * Rama de funcionalidad activa: `feature/pdf-export`.
   * **Pull Request #1 en vivo:** [https://github.com/Bryd3n/ISII-Everything-as-Code-Demo/pull/1](https://github.com/Bryd3n/ISII-Everything-as-Code-Demo/pull/1) con su plantilla técnica formal de descripción, evaluación de impacto y checklist de revisión.
2. **Everything as Code & Contenedorización Inmutable (Ejercicio 2 / Brayan Carreño):**
   * Microservicio modular Node.js / Express en puerto 8080 con endpoints de salud `/health` y facturación `/api/facturas`.
   * `Dockerfile` multi-etapa optimizado que erradica la deriva de configuración (*Configuration Drift*) ejecutando como usuario no-root.
3. **Pipeline de Integración Continua (CI & 3 Quality Gates):**
   * Automatización en GitHub Actions (`.github/workflows/ci.yml`) validando en verde:
     - **Gate 1:** Pruebas unitarias automatizadas (`npm test`).
     - **Gate 2:** Auditoría de seguridad de dependencias (`npm audit`).
     - **Gate 3:** Compilación y empaquetado del contenedor Docker.
4. **Orquestación Declarativa (Pregunta 4 / Brayan Carreño):**
   * Manifiestos versionados `.gitignore`, `Dockerfile`, `.dockerignore`, `.github/workflows/ci.yml` y `docker-compose.yml`.

---

### 2. Video de la Defensa Oral (Google Drive)
* **Enlace de Google Drive:** *(Pendiente de enlazar tras la compilación del video final del equipo)*

---

## 📂 Directorio de Entregables por Integrante

### 📌 Integrante 1: Rhixeidys Aguilera
* **Carpeta:** `01_Pregunta_1_Flujo_Git_Hotfix_y_CI/`
* **Lámina de Defensa (16:9 Dark Theme):** `01_Lamina_Defensa_Ejercicio_1_Rhixeidys.png` *(con espacio superior libre para cámara OBS)*
* **Lámina HTML Interactiva:** `01_Pregunta_1_Flujo_Git_Hotfix_y_CI/Laminas_y_Diapositivas/01_Lamina_Defensa_Ejercicio_1_Rhixeidys.html`
* **Guión de Exposición Oral:**
  - Formato Word: `01_Pregunta_1_Flujo_Git_Hotfix_y_CI/Guiones_de_Defensa/Guion_Defensa_Ejercicio_1_Rhixeidys.docx`
  - Formato Markdown: `01_Pregunta_1_Flujo_Git_Hotfix_y_CI/Guiones_de_Defensa/Guion_Defensa_Ejercicio_1_Rhixeidys.md`

### 📌 Integrante 2: Yonkeiner Bravo
* **Carpeta:** `02_Pregunta_2_GitFlow_vs_TrunkBased/`
* **Lámina de Defensa (16:9 Dark Theme):** `01_Lamina_Defensa_Pregunta_2_Yonkeiner.png` *(con espacio superior libre para cámara OBS)*
* **Lámina HTML Interactiva:** `02_Pregunta_2_GitFlow_vs_TrunkBased/Laminas_y_Diapositivas/01_Lamina_Defensa_Pregunta_2_Yonkeiner.html`
* **Guión de Exposición Oral:**
  - Formato Word: `02_Pregunta_2_GitFlow_vs_TrunkBased/Guiones_de_Defensa/Guion_Defensa_Pregunta_2_Yonkeiner.docx`
  - Formato Markdown: `02_Pregunta_2_GitFlow_vs_TrunkBased/Guiones_de_Defensa/Guion_Defensa_Pregunta_2_Yonkeiner.md`

### 📌 Integrante 4: Brayan Carreño
* **Carpeta:** `04_Ejercicio_2_y_Pregunta_4_Everything_as_Code/`
* **Informe Formal Académico:** `Ejercicio_2_y_Pregunta_4_Brayan.pdf` (con portada institucional UNEG)
* **Lámina de Defensa (16:9 Dark Theme):** `01_Lamina_Defensa_Ejercicio_2_y_Pregunta_4_Brayan.png` *(con espacio superior libre para cámara OBS)*
* **Guión de Exposición Oral:**
  - Formato Word: `04_Ejercicio_2_y_Pregunta_4_Everything_as_Code/Guiones_de_Defensa/Guion_Defensa_Ejercicio_2_y_Pregunta_4.docx`
  - Formato Markdown: `04_Ejercicio_2_y_Pregunta_4_Everything_as_Code/Guiones_de_Defensa/Guion_Defensa_Ejercicio_2_y_Pregunta_4.md`
* **Código Fuente y Configuración en Vivo:** [https://github.com/Bryd3n/ISII-Everything-as-Code-Demo](https://github.com/Bryd3n/ISII-Everything-as-Code-Demo)
