# Guión de Defensa Oral – Ejercicio 1 (Pregunta 1)
**Unidad V: Gestión de Configuración, Versionamiento y DevOps**  
**Asignatura:** Ingeniería de Software II – 7mo Semestre (UNEG)  
**Profesor:** Mg. Félix Márquez  
**Presentadora:** Rhixeidys Aguilera  
**Equipo:** Ingenio y Código  
**Duración Estimada:** 2 minutos 15 segundos (~340 palabras)  
**Lámina de Apoyo:** `01_Lamina_Defensa_Ejercicio_1_Rhixeidys.png`

---

### Estructura y Distribución de Tiempos

| Bloque | Tiempo | Tema | Enfoque Clave |
| :--- | :---: | :--- | :--- |
| **I. Introducción** | 00:00 - 00:25 | Presentación y Planteamiento del Incidente | Contexto del desarrollo concurrente y la emergencia en producción. |
| **II. Bloque 1: Git Workflow** | 00:25 - 01:05 | Secuencia Técnica de Comandos Git | Aislamiento con `stash`, ramificación limpia, hotfix y rebase para evitar merge hell. |
| **III. Bloque 2: Pull Request** | 01:05 - 01:40 | Estándar de Plantilla de Pull Request | Descripción técnica, evaluación de impacto y checklist humano. |
| **IV. Bloque 3: Quality Gates** | 01:40 - 02:15 | Puertas de Calidad en Pipeline de CI | Los 3 Gates: Cobertura lógica (80%), Calidad SAST y Seguridad SCA. |

---

### Guión de Exposición (Lectura en Primera Persona)

#### [00:00 - 00:25] Introducción y Planteamiento del Incidente
> *"Saludos, profesor Félix Márquez y compañeros. Mi nombre es **Rhixeidys Aguilera**, y en esta defensa abordaré el **Ejercicio 1**, enfocado en la gestión profesional de configuración, resolución de incidentes en producción mediante Git y el diseño de políticas rigurosas de integración continua.*
>
> *El escenario planteado simula una situación clásica en la industria: mientras nos encontramos a mitad del desarrollo de una funcionalidad crítica —la exportación de facturas en PDF—, surge un error bloqueante en el login de producción que requiere remediación inmediata."*

#### [00:25 - 01:05] Bloque 1: Gestión de Flujo Git ante Incidentes
*(Señalar la columna 1 de la lámina)*
> *"Para resolver esto sin perder trabajo ni ensuciar el historial, implementamos una estrategia de 4 fases:*
>
> 1. *Primero, ejecutamos `git stash push` con un mensaje descriptivo. Esto resguarda de forma segura nuestros cambios locales no confirmados sin generar commits basura en el árbol.*
> 2. *Segundo, nos movemos a la rama principal con `git checkout main`, actualizamos el estado remoto con `git pull` y creamos la rama de emergencia `hotfix/login-bug`.*
> 3. *Tercero, una vez corregida la autenticación, confirmamos el parche con un commit semántico, lo publicamos con `git push` y generamos el despliegue a producción.*
> 4. *Y cuarto, para regresar a nuestra funcionalidad, ejecutamos `git checkout feature/pdf-export` y aplicamos un `git rebase origin/main`. Al usar rebase en lugar de merge, reescribimos nuestra rama sobre la base del parche de producción, manteniendo un historial lineal y limpio, para finalmente recuperar nuestros cambios con `git stash pop`."*

#### [01:05 - 01:40] Bloque 2: Plantilla de Pull Request Profesional
*(Señalar la columna central de la lámina)*
> *"En la columna central observamos nuestra **Plantilla de Pull Request**. El objetivo del PR no es solo solicitar código, sino ser un documento de trazabilidad y gobernanza.*
>
> *Estructuramos la plantilla en tres secciones fundamentales:*
> * *La **Descripción Técnica**, donde se especifica el endpoint intervenido —en este caso `/api/facturas/:id/pdf`— y la librería PDF seleccionada.*
> * *La **Evaluación de Impacto**, donde analizamos el consumo de memoria en el motor V8 al procesar streams de datos y garantizamos el blindaje contra inyecciones.*
> * *Y una **Checklist de Verificación Humana**, que obliga al desarrollador a validar la existencia de pruebas unitarias, escaneo de dependencias y la ejecución contenerizada como usuario no-root."*

#### [01:40 - 02:15] Bloque 3: Quality Gates en el Pipeline de CI
*(Señalar la columna 3 de la lámina)*
> *"Finalmente, establecemos tres **Quality Gates** automáticos en GitHub Actions que actúan como árbitros algorítmicos:*
>
> * *El **Gate 1** valida la integridad lógica mediante `npm test`, exigiendo un umbral mínimo de cobertura del 80%. Si una sola prueba falla, el pipeline bloquea la integración.*
> * *El **Gate 2** realiza análisis estático de código con herramientas SAST como SonarQube, detectando code smells, duplicidad y complejidad ciclomática excesiva.*
> * *Y el **Gate 3** ejecuta un escaneo de composición de software mediante `npm audit`, asegurando que ninguna dependencia de terceros introduzca vulnerabilidades CVE en el producto.*
>
> *Con estos tres filtros y la aprobación humana obligatoria, garantizamos que solo código seguro, probado y de alta mantenibilidad alcance la rama principal. Muchas gracias."*
