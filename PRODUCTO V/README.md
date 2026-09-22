# PRODUCTO V: Gestión de Configuración, Versionamiento y DevOps
### Universidad Nacional Experimental de Guayana (UNEG)
**Asignatura:** Ingeniería de Software II – Prof. Mg. Félix Márquez  
**Equipo:** *Ingenio y Código*  

---

## 🔗 Repositorio Oficial del Proyecto de la Unidad V

Tal como se estipula en las pautas de evaluación para la entrega del Producto V, se coloca la dirección del repositorio del proyecto en el cual se realizó la implementación técnica y el flujo de integración continua:

👉 **Repositorio del Proyecto:**  
[https://github.com/Bryd3n/ISII-Everything-as-Code-Demo](https://github.com/Bryd3n/ISII-Everything-as-Code-Demo)

👉 **Pull Request #1 de Evaluación en Vivo (Rama `feature/pdf-export`):**  
[https://github.com/Bryd3n/ISII-Everything-as-Code-Demo/pull/1](https://github.com/Bryd3n/ISII-Everything-as-Code-Demo/pull/1)

---

### 🛠️ Implementaciones Técnicas en el Repositorio:
* **Everything as Code & Contenedorización Inmutable:** Microservicio modular en Node.js / Express con `Dockerfile` multi-etapa optimizado que erradica la deriva de configuración (*Configuration Drift*).
* **Pipeline de Integración Continua (CI & Quality Gates):** Automatización en GitHub Actions (`.github/workflows/ci.yml`) validando en verde los 3 Quality Gates (pruebas unitarias automatizadas, auditoría de seguridad `npm audit` y empaquetado Docker).
* **Flujo Git & Plantilla Formal de Pull Request:** Implementación de GitHub Flow con plantilla estructurada de descripción técnica, evaluación de impacto y checklist de revisión humana.
* **Orquestación Declarativa:** Manifiestos versionados `.gitignore`, `Dockerfile`, `.dockerignore`, `.github/workflows/ci.yml` y `docker-compose.yml`.
