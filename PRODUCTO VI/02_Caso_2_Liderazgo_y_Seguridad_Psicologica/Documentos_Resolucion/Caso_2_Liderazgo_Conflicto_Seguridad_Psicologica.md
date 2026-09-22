# UNIVERSIDAD NACIONAL EXPERIMENTAL DE GUAYANA
### Vicerrectorado Académico | Coordinación de Ingeniería en Informática
**Asignatura:** Ingeniería de Software II – 7mo Semestre  
**Profesor:** Mg. Félix Márquez  
**Unidad VI:** Liderazgo, Equipos y Cultura de Ingeniería  
**Caso 2:** Liderazgo, Conflicto y Seguridad Psicológica  
**Autores del Caso:** Brayan Carreño (Integrante 3) y Nicole García (Integrante 4)  
**Equipo:** Ingenio y Código  
**Fecha de Entrega:** 23/09/2026  

---

## 📖 Planteamiento del Caso 2
> **Contexto:**  
> *«Usted es el nuevo Agile Coach / Líder Técnico de un equipo. Nota que en las revisiones de código (Pull Requests), el Arquitecto Principal (un desarrollador muy senior y brillante) utiliza comentarios sarcásticos y destructivos hacia los desarrolladores junior, tales como: "¿En serio vas a usar este patrón? Es de principiantes". Los juniors han dejado de proponer ideas en las retrospectivas y la velocidad de entrega ha caído.»*

---

## 🧠 PARTE A: Diagnóstico de Seguridad Psicológica y Abordaje del Conflicto
**Responsable:** Brayan Carreño (Integrante 3)

### 1. Diagnóstico de la Situación utilizando la Seguridad Psicológica (Amy Edmondson)

#### 1.1. Marco Teórico: El Constructo de Seguridad Psicológica
La **Dra. Amy Edmondson (1999)** define la Seguridad Psicológica (*Psychological Safety*) como la creencia compartida por los miembros de un equipo de que el entorno es seguro para la toma de riesgos interpersonales. En un equipo con alta seguridad psicológica, las personas confían en que nadie será humillado, ridiculizado, sancionado o marginado por:
1. Hacer preguntas cuando no entienden un concepto.
2. Admitir errores o desconocimiento ante una tecnología.
3. Proponer ideas divergentes o soluciones arquitectónicas innovadoras.
4. Señalar fallos en el código o en los procesos establecidos.

Esta premisa fue ratificada empíricamente por Google en su investigación de cinco años denominada **Proyecto Aristotle (2015)**. Tras analizar cientos de equipos de ingeniería, Google concluyó que la seguridad psicológica no es solo un factor positivo de convivencia, sino el **predictor estadístico número uno (#1) indiscutible del alto rendimiento y la excelencia en ingeniería de software**, por encima de la antigüedad promedio, la brillantez individual o los presupuestos asignados.

#### 1.2. Diagnóstico del Equipo: Desplazamiento a la "Zona de Ansiedad"
Según el modelo de cuatro cuadrantes de Edmondson (que cruza los *Estándares de Rendimiento* con la *Seguridad Psicológica*):

```
       Alta Seguridad Psicológica
                   ▲
  Zona de Confort  │  Zona de Aprendizaje
  (Bajo reto,      │  y Alto Rendimiento
   sin miedo)      │  (Meta del Equipo)
───────────────────┼────────────────────► Altos Estándares
   Zona de Apatía  │  Zona de Ansiedad
  (Desmotivación,  │  (Terror al ridículo,
   silencio total) │  parálisis técnica)
                   │
       Baja Seguridad Psicológica
```

1. **Estado Actual:** El equipo posee altos estándares técnicos (impuestos por la figura del Arquitecto Principal), pero la seguridad psicológica ha sido severamente destruida por sus comentarios sarcásticos (*«¿En serio vas a usar este patrón? Es de principiantes»*).
2. **Consecuencia Inmediata:** El equipo ha caído en la **Zona de Ansiedad**, mutando rápidamente hacia la **Zona de Apatía**. Cuando un profesional junior es objeto de burla pública en una plataforma colaborativa como GitHub/GitLab, el cerebro activa respuestas de amenaza social (amígdala cerebral), inhibiendo la creatividad, el razonamiento analítico y la iniciativa.
3. **Efecto de Silencio Colectivo:** Los desarrolladores juniors aplican una estrategia defensiva de autopreservación: *el silencio*. Dejar de opinar en las retrospectivas no es falta de interés, sino el mecanismo más racional para evitar ser humillados públicamente.

#### 1.3. Impacto en el Rendimiento del Equipo a Largo Plazo
Si esta disfunción cultural no se interviene de inmediato, el impacto técnico y operativo sobre el sistema es devastador:

* **Ocultamiento Sistemático de Errores y Deuda Técnica:** Al imperar el miedo al escarnio, los desarrolladores evitan reportar fallos tempranos, dudas conceptuales o malas decisiones de diseño. Prefieren "parchar" el código a escondidas, lo que engendra *bugs* silenciosos y una deuda técnica catastrófica que estalla en producción (el llamado "Efecto Chernobyl" en software).
* **Colapso de las Métricas DORA (*Accelerate*):**
  * *Lead Time for Changes:* Se dilata de horas a semanas porque los desarrolladores retrasan el envío de Pull Requests por pánico a la revisión del arquitecto.
  * *Change Failure Rate:* Aumenta sustancialmente debido a la falta de discusión abierta sobre casos borde y validaciones de seguridad.
* **Parálisis por Análisis y Muerte de la Innovación:** Se extingue la experimentación. Los desarrolladores optan por copiar y pegar patrones antiguos obsoletos que el arquitecto ya haya aprobado previamente, aunque no sean los más idóneos, evitando proponer enfoques modernos.
* **Fuga de Talento y Destrucción del Clima:** Pérdida acelerada de desarrolladores juniors y de nivel medio. Los costos de reclutamiento, inducción y pérdida de conocimiento de dominio superan con creces el valor de la brillantez técnica aislada del arquitecto.

---

### 2. Estrategia de Intervención con Liderazgo de Servicio y Comunicación No Violenta

#### 2.1. Marco de Liderazgo: De "Comando y Control" a Liderazgo Servicial y Adaptativo
Como nuevo Agile Coach / Tech Lead, no se debe responder con una sanción punitiva o una confrontación de egos, ya que el Arquitecto es una pieza técnica valiosa. Siguiendo el **Liderazgo de Servicio** (*Robert Greenleaf, 1977*) y el **Liderazgo Adaptativo** (*Ronald Heifetz, 2009*), el rol del líder es remover impedimentos sistémicos y ayudar al arquitecto a transitar desde un *experto técnico solitario* hacia un *líder multiplicador y mentor*.

#### 2.2. Guión de Conversación en Privado con el Arquitecto Principal (Modelo CNV)
La reunión se realiza en un espacio privado (1 a 1), aplicando rigurosamente los cuatro pasos de la **Comunicación No Violenta (CNV)** desarrollada por **Marshall Rosenberg**:

1. **Paso 1: Observación de Hechos Concretos (Sin Juicios ni Etiquetas):**
   > *«Hola [Nombre del Arquitecto]. Te invité a este espacio porque valoro profundamente tu excelencia técnica y tu rol central en la arquitectura de nuestros sistemas. Revisando los Pull Requests de esta semana, observé este comentario textual en el PR #48 del módulo de pagos: "¿En serio vas a usar este patrón? Es de principiantes".»*  
   *(Se describe el hecho específico sin adjetivos como "fuiste grosero" o "eres tóxico").*

2. **Paso 2: Expresión de Sentimientos y Preocupación por el Ecosistema:**
   > *«Al leer ese comentario y notar que en las dos últimas retrospectivas los juniors guardaron silencio absoluto y la velocidad de cierre de historias bajó un 30%, me siento sumamente preocupado por la sostenibilidad del equipo y por el ambiente de confianza que necesitamos consolidar.»*

3. **Paso 3: Identificación de Necesidades Compartidas:**
   > *«Sé que para ti es fundamental mantener un estándar de código impecable, escalable y sin errores en producción; esa es una necesidad que comparto plenamente contigo. Sin embargo, para que el proyecto escale sin que tú tengas que revisar línea por línea, necesitamos que el equipo aprenda, se equivoque rápido sin miedo y desarrolle autonomía técnica. La excelencia técnica requiere un ambiente seguro para florecer.»*

4. **Paso 4: Petición Concreta, Operacionalizable y Negociable:**
   > *«Quiero pedirte dos cosas puntuales:*  
   > *1. Que en los comentarios de código sustituyamos los juicios de valor por preguntas orientadoras y ejemplos concretos. En lugar de señalar que un patrón es de novatos, explicar por qué ese patrón tiene problemas de concurrencia o memoria en este caso puntual y sugerir la alternativa.*  
   > *2. Que me ayudes a co-diseñar una guía de revisión de Pull Requests y a automatizar reglas en el pipeline para que los linters filtren la sintaxis y tú puedas enfocar tu tiempo en mentorías de alto nivel.*  
   > *¿Cómo lo ves y cómo podemos trabajar juntos en esto?»*

---

## 🛠️ PARTE B: Reestructuración de Pull Requests y Dinámica de Retrospectiva
**Responsable:** Nicole García (Integrante 4)

### 3. Reestructuración del Proceso de Revisión de Código (Pull Requests)

Para que el cambio no dependa únicamente de la buena voluntad, se debe rediseñar el proceso técnico eliminando la fricción y despersonalizando el feedback:

#### 3.1. Despersonalización mediante Automatización en CI (Quality Gates)
Las discusiones subjetivas sobre estilo, formato, sangrías o malas prácticas comunes deben ser delegadas a herramientas automáticas antes de que un humano abra el PR:
* **Formateadores Automáticos y Linters (Prettier, ESLint, Checkstyle):** Integrados en hooks locales (`pre-commit`) y en el pipeline de CI. Si un archivo no cumple el estándar de formato, el commit es rechazado algorítmicamente.
* **Análisis Estático de Código (SAST / SonarQube):** Evalúa complejidad ciclomática, duplicación de código, cobertura de pruebas y vulnerabilidades de seguridad de forma matemática y neutra.
* **Principio de Despersonalización:** *"Los linters y analizadores juzgan el formato y los errores comunes; los ingenieros debaten la arquitectura, la lógica de negocio y la legibilidad."* Esto erradica el 70% de las fricciones en revisiones.

#### 3.2. Estandarización de Feedback: Adopción de *Conventional Comments*
Se establece como política institucional obligatoria el estándar internacional de **Conventional Comments** ([conventionalcomments.org](https://conventionalcomments.org)). Todo comentario humano en un Pull Request debe incluir un prefijo semántico que explicita la intención y el nivel de exigencia:

| Etiqueta Semántica | Significado / Intención | Ejemplo de Aplicación Constructiva |
| :--- | :--- | :--- |
| **`praise:`** | Elogio sincero por una solución elegante o bien probada. Refuerza positivamente el aprendizaje. | `praise: Excelente manejo del desacoplamiento en este adaptador de pagos. Es muy legible.` |
| **`suggestion:`** | Propuesta de mejora técnica opcional o recomendada. Requiere justificación y código de ejemplo. | `suggestion (no-bloqueante): Considera usar el patrón Factory aquí para evitar el switch múltiple. Te dejo este snippet: [...]` |
| **`issue:`** | Problema real funcional, de seguridad o rendimiento que **bloquea** el merge. Debe explicarse el porqué. | `issue (bloqueante): Este bucle ejecuta consultas SQL dentro de una iteración (N+1). Puede causar saturación en la BD con más de 100 registros.` |
| **`question:`** | Pregunta genuina para comprender la intención del autor, sin asumir un fallo. | `question: ¿Por qué elegiste un bloqueo síncrono en lugar de un canal asíncrono para este procesamiento? Me gustaría entender el caso de uso.` |
| **`thought:`** | Reflexión o idea para discutir en el futuro, no aplicable de inmediato al PR actual. | `thought: A futuro podríamos desacoplar esta validación en un microservicio independiente.` |
| **`nitpick:`** | Detalle menor de pulido que no impide el despliegue a producción. | `nitpick: Podríamos renombrar esta variable a 'esValido' para mayor claridad semántica.` |

#### 3.3. Código de Conducta en Revisiones de Código (*Code Review Charter*)
Se formaliza un acuerdo de equipo con tres reglas de oro:
1. **Criticar el código, jamás a la persona:** Prohibido el uso de sarcasmo, descalificaciones o adjetivos personales.
2. **Toda crítica debe incluir una alternativa:** Quien señale un defecto está obligado a sugerir cómo resolverlo o brindar una referencia documental.
3. **Revisión en menos de 4 horas y PRs pequeños (< 400 líneas):** Facilita revisiones ágiles y pedagógicas.

---

### 4. Dinámica Práctica para la Próxima Retrospectiva: "Reconstruyendo la Confianza"

Para sanar la fractura emocional y recuperar la participación activa de los desarrolladores juniors, se diseña una sesión de Retrospectiva estructurada de 60 minutos en tres fases:

#### 4.1. Fase 1: *Safety Check* Anónimo (10 minutos)
Inspirado en el marco de **Derby & Larsen (2006)** para facilitar retrospectivas ágiles:
* **Mecánica:** Antes de entrar en materia, cada integrante vota de forma 100% anónima en una herramienta digital (Menti o tablero anónimo) asignándose un puntaje del 1 al 5 según su nivel de seguridad psicológica percibida:
  * **1 (Terror):** *"No pienso hablar; todo lo que diga puede ser usado en mi contra."*
  * **2 (Cauto):** *"Solo hablaré si es estrictamente necesario y seguro."*
  * **3 (Neutral):** *"Participaré en temas normales, pero no en temas conflictivos."*
  * **4 (Abierto):** *"Me siento cómodo hablando de la mayoría de las dificultades."*
  * **5 (Plena Confianza):** *"Hablo con total libertad, asumo riesgos y propongo sin temor."*
* **Propósito:** Visibilizar de forma objetiva y colectiva la temperatura emocional del equipo. Si el promedio está por debajo de 3.5, el facilitador suspende la agenda ordinaria para dedicarse exclusivamente a hablar de la convivencia y el apoyo mutuo.

#### 4.2. Fase 2: Dinámica Central *Reconocimiento Cruzado & Círculo de Aprendizaje* (35 minutos)
Se implementa una adaptación de la técnica **"Hero, Highlight & Hardship"** combinada con **"Kudo Cards"**:
1. **Parte 1 (Reconocimiento Cruzado Obligatorio):**
   * Cada miembro del equipo (comenzando por el Facilitador y el Arquitecto Principal) debe entregar una tarjeta de agradecimiento pública (*Kudo*) a otro compañero, destacando una ayuda técnica, una paciencia demostrada o una idea valiosa aportada en el sprint.
   * *Acción facilitadora:* Se invita explícitamente al Arquitecto a reconocer el esfuerzo y la evolución de los desarrolladores juniors, validando su progreso ante todo el equipo.
2. **Parte 2 (Normalización del Error como Motor de Ingeniería):**
   * El Líder Técnico / Agile Coach expone un error técnico grave propio cometido en el pasado (vulnerabilidad de seguridad, caída de servidor) para modelar la vulnerabilidad.
   * Se debate la premisa: *"En este equipo no buscamos culpables individuales ante los fallos; buscamos debilidades en nuestros tests y procesos de automatización."*

#### 4.3. Fase 3: Co-creación del *Team Working Agreement* (15 minutos)
* El equipo redacta y vota colectivamente sus **Acuerdos de Convivencia y Mentoría**.
* Se plasman en un documento vivo versionado en el repositorio (ej. `WORKING_AGREEMENT.md`) con compromisos explícitos sobre el uso de *Conventional Comments*, el respeto en los PRs y el soporte colaborativo diario.
* **Cierre:** Compromiso explícito de cada miembro con un apretón de manos simbólico y monitoreo de las métricas en las siguientes dos semanas.

---

## 📚 Referencias Bibliográficas
1. **Edmondson, A. C. (1999).** *Psychological Safety and Learning Behavior in Work Teams.* Administrative Science Quarterly, 44(2), 350-383.
2. **Edmondson, A. C. (2018).** *The Fearless Organization: Creating Psychological Safety in the Workplace for Learning, Innovation, and Growth.* John Wiley & Sons.
3. **Forsgren, N., Humble, J., & Kim, G. (2018).** *Accelerate: The Science of Lean Software and DevOps: Building and Scaling High Performing Technology Organizations.* IT Revolution Press.
4. **Greenleaf, R. K. (1977).** *Servant Leadership: A Journey into the Nature of Legitimate Power and Greatness.* Paulist Press.
5. **Heifetz, R., Grashow, A., & Linsky, M. (2009).** *The Practice of Adaptive Leadership: Tools and Tactics for Changing Your Organization and the World.* Harvard Business Press.
6. **Rosenberg, M. B. (2015).** *Nonviolent Communication: A Language of Life* (3rd ed.). PuddleDancer Press.
7. **Derby, E., & Larsen, D. (2006).** *Agile Retrospectives: Making Good Teams Great.* Pragmatic Bookshelf.
8. **Duhigg, C. (2016).** *What Google Learned From Its Quest to Build the Perfect Team (Project Aristotle).* The New York Times Magazine.
