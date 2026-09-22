# Guión de Defensa Oral – Caso 2 (Parte B)
**Unidad VI: Liderazgo, Equipos y Cultura de Ingeniería**  
**Asignatura:** Ingeniería de Software II – 7mo Semestre (UNEG)  
**Profesor:** Mg. Félix Márquez  
**Presentadora:** Nicole García (Integrante 4)  
**Equipo:** Ingenio y Código  
**Duración Estimada:** 2 minutos 20 segundos (~360 palabras)  
**Lámina de Apoyo:** `02_Lamina_Defensa_Caso_2_Nicole.png`

---

### Estructura y Distribución de Tiempos

| Bloque | Tiempo | Tema | Enfoque Clave |
| :--- | :---: | :--- | :--- |
| **I. Introducción** | 00:00 - 00:25 | Presentación y Conexión | Solución técnica y metodológica para despersonalizar el feedback y reconstruir la confianza. |
| **II. Automatización en CI** | 00:25 - 00:55 | Despersonalización mediante Quality Gates | Linters (Prettier, ESLint) y SonarQube: «Las máquinas revisan el estilo; los humanos la arquitectura». |
| **III. Conventional Comments** | 00:55 - 01:35 | Estandarización y Código de Conducta | Etiquetas semánticas (`praise:`, `suggestion:`, `issue:`), crítica objetiva y PRs pequeños (< 400 líneas). |
| **IV. Retrospectiva Segura** | 01:35 - 02:20 | Dinámica de Restauración de Confianza | Safety Check anónimo (Derby & Larsen), Kudo Cards con el arquitecto y Team Working Agreement. |

---

### Guión de Exposición (Lectura en Primera Persona)

#### [00:00 - 00:25] Introducción: De la Intervención Humana a la Solución Sistémica
> *"Saludos cordiales, profesor Félix Márquez y compañeros. Mi nombre es **Nicole García**, y como **Integrante 4** me corresponde presentar la **Parte B del Caso 2: Reestructuración de Pull Requests y Restauración de la Confianza**.*
>
> *Complementando el abordaje en privado expuesto por mi compañero Brayan Carreño, mi responsabilidad como líder es garantizar que el cambio cultural no dependa solo de buenas intenciones, sino de un rediseño de nuestros procesos y herramientas de ingeniería para blindar la seguridad psicológica del equipo."*

#### [00:25 - 00:55] Bloque 1: Despersonalización del Feedback mediante CI
*(Señalar la columna 1 de la lámina)*
> *"En la primera columna aplicamos el principio fundamental de despersonalización:*
>
> * Gran parte de los roces en revisiones nacen de discusiones subjetivas sobre formato, sangrías o malas prácticas elementales. Por ello, delegamos esa carga a herramientas automáticas: configuramos **linters y formateadores (como Prettier y ESLint)** en hooks de pre-commit y **análisis estático con SonarQube** en el pipeline de Integración Continua.
> * Establecemos como axioma de equipo: *'Las máquinas evalúan el estilo y los errores comunes; los humanos debatimos la arquitectura, el diseño y la lógica de negocio'*. Si el commit viola una regla sintáctica, es rechazado algorítmicamente sin que intervenga el ego de ningún colega."*

#### [00:55 - 01:35] Bloque 2: Conventional Comments y Protocolo de Revisión
*(Señalar las columnas 2 y 3 de la lámina)*
> *"En la segunda y tercera columna estandarizamos la comunicación humana mediante el estándar internacional de **Conventional Comments**.*
>
> *A partir de ahora, todo comentario en un Pull Request debe incluir un prefijo semántico que explicita su intención:*
> * `praise:` para elogiar públicamente un código limpio y reforzar el aprendizaje;
> * `suggestion:` para proponer mejoras no bloqueantes acompañadas de un snippet de ejemplo;
> * e `issue:` reservado estrictamente para bugs o fallas de concurrencia y seguridad que bloquean el merge, siempre con justificación técnica.
>
> *Esto se complementa con un **Protocolo de Revisión**: prohibición absoluta del sarcasmo, obligación de sugerir alternativas viables ante cada observación y el compromiso de mantener **Micro-PRs de menos de 400 líneas** revisados en menos de 4 horas."*

#### [01:35 - 02:20] Bloque 3: Dinámica de Retrospectiva para Reconstruir la Confianza
*(Señalar la columna 4 de la lámina)*
> *"Finalmente, en la cuarta columna diseñamos una **Retrospectiva estructurada de 60 minutos** para sanar la relación del equipo:*
>
> 1. *Iniciamos con un **Safety Check anónimo** de 10 minutos (siguiendo a Derby y Larsen), donde cada integrante califica del 1 al 5 su grado de seguridad para hablar, visibilizando la salud emocional colectiva.*
> 2. *Pasamos a una dinámica de **Kudo Cards y Reconocimiento Cruzado** de 35 minutos, donde invitamos de forma protagonista al Arquitecto Principal a reconocer públicamente el esfuerzo y las soluciones aportadas por los juniors.*
> 3. *Y cerramos con la co-creación de un **Team Working Agreement** de 15 minutos, un acuerdo formal de convivencia técnica que firma todo el equipo y que se versiona en la raíz de nuestro repositorio.*
>
> *Con estas medidas, transformamos un conflicto destructivo en un entorno de alto desempeño, aprendizaje continuo y respeto mutuo. Muchas gracias."*
