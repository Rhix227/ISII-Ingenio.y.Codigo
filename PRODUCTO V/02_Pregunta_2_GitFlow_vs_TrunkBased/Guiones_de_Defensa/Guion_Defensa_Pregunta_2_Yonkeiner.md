# Guión de Defensa Oral – Pregunta 2
**Unidad V: Gestión de Configuración, Versionamiento y DevOps**  
**Asignatura:** Ingeniería de Software II – 7mo Semestre (UNEG)  
**Profesor:** Mg. Félix Márquez  
**Presentador:** Yonkeiner Bravo  
**Equipo:** Ingenio y Código  
**Duración Estimada:** 2 minutos 25 segundos (~365 palabras)  
**Lámina de Apoyo:** `01_Lamina_Defensa_Pregunta_2_Yonkeiner.png`

---

### Estructura y Distribución de Tiempos

| Bloque | Tiempo | Tema | Enfoque Clave |
| :--- | :---: | :--- | :--- |
| **I. Introducción** | 00:00 - 00:25 | Presentación del Paradigma de Entrega | Cambio de paradigma: software en caja vs. DevOps cloud-native. |
| **II. Bloque 1: Branching** | 00:25 - 00:55 | GitFlow vs. Trunk-Based Development | Ramas largas y Merge Hell vs. integración diaria en trunk con ramas efímeras. |
| **III. Bloque 2: DORA Metrics** | 00:55 - 01:30 | Evidencia Empírica de *Accelerate* | Las 4 métricas DORA: Frecuencia, Lead Time, MTTR y Change Failure Rate. |
| **IV. Bloque 3: Prácticas TBD** | 01:30 - 02:00 | Feature Flags y Micro-PRs | Desacoplar Despliegue de Liberación y pipelines de CI veloces. |
| **V. Bloque 4: Despliegue CD** | 02:00 - 02:25 | Estrategias Zero-Downtime | Blue/Green, Canary Releases y Rolling Updates. |

---

### Guión de Exposición (Lectura en Primera Persona)

#### [00:00 - 00:25] Introducción: De la Era Tradicional a la Era Cloud-Native
> *"Saludos cordiales, profesor Félix Márquez y compañeros. Mi nombre es **Yonkeiner Bravo**, y me corresponde exponer la **Pregunta 2**, donde contrastamos dos filosofías de entrega de software: el modelo tradicional **GitFlow** frente a **Trunk-Based Development**, respaldado por la evidencia empírica del libro *Accelerate* y las estrategias avanzadas de Despliegue Continuo.*
>
> *Hoy en día, la velocidad y la estabilidad ya no son excluyentes: son el estándar de la ingeniería de software de alto desempeño."*

#### [00:25 - 00:55] Bloque 1: Modelos de Branching (GitFlow vs. TBD)
*(Señalar la columna 1 de la lámina)*
> *"En la primera columna comparamos ambos enfoques:*
>
> * **GitFlow** nació para la era del software en cajas con releases trimestrales. Utiliza múltiples ramas de larga duración como `develop`, `release` y `feature`. Su gran debilidad es el infame **Merge Hell**: cuando los desarrolladores pasan semanas aislados en sus ramas, integrar el código resulta traumático y propenso a errores.
> * Frente a esto, **Trunk-Based Development** es el estándar moderno en la nube. Aquí, todos los desarrolladores integran su trabajo a la rama principal —el *trunk*— al menos **una vez al día**, usando ramas efímeras de menos de 24 o 48 horas. Esto elimina los conflictos destructivos y proporciona retroalimentación inmediata."*

#### [00:55 - 01:30] Bloque 2: La Evidencia de *Accelerate* y las Métricas DORA
*(Señalar la columna 2 de la lámina)*
> *"En la columna dos vemos que esto no es una moda, sino ciencia empírica comprobada. Las investigaciones de Nicole Forsgren, Jez Humble y Gene Kim demostraron estadísticamente que Trunk-Based Development es un predictor directo del éxito organizacional.*
>
> *Ellos definieron las cuatro métricas **DORA**:*
> 1. *La **Frecuencia de Despliegue**, donde los equipos élite despliegan múltiples veces al día a demanda.*
> 2. *El **Lead Time**, o tiempo desde el commit hasta producción, que se reduce a menos de una hora frente a los meses de los equipos tradicionales.*
> 3. *El **MTTR**, logrando restaurar servicios tras un incidente en menos de una hora.*
> 4. *Y la **Tasa de Falla en Cambios**, que se mantiene entre el 0 y el 15%, desmintiendo el mito de que desplegar rápido rompe el sistema."*

#### [01:30 - 02:00] Bloque 3: Prácticas Clave en TBD y Feature Flags
*(Señalar la columna 3 de la lámina)*
> *"¿Cómo logramos integrar código incompleto a diario sin romper producción? Mediante las prácticas de la tercera columna:*
>
> * La técnica reina son los **Feature Flags** o conmutadores de funcionalidad. Como vemos en el código de ejemplo, el Feature Flag nos permite **desacoplar el despliegue de la liberación**. El código de una nueva función se instala en el servidor en producción, pero permanece apagado para los usuarios hasta que esté 100% maduro.
> * Esto se complementa con **Micro-Pull Requests** de menos de 400 líneas y un pipeline de Integración Continua que responde en menos de 10 minutos."*

#### [02:00 - 02:25] Bloque 4: Estrategias Avanzadas de Despliegue Continuo (Zero-Downtime)
*(Señalar la columna 4 de la lámina)*
> *"Finalmente, en la cuarta columna implementamos despliegues con cero tiempo de inactividad:*
>
> * **Blue/Green Deployment**, donde mantenemos dos entornos idénticos y el enrutador conmuta el 100% del tráfico instantáneamente, permitiendo un rollback en milisegundos si algo sale mal.
> * **Canary Releases**, exponiendo la nueva versión progresivamente a un 5% de usuarios, evaluando latencia y errores antes de escalar al 100%.
> * Y los **Rolling Updates**, actualizando réplicas gradualmente en clústeres como Kubernetes.
>
> *En conclusión, Trunk-Based Development junto a estas estrategias de CD transforma la entrega de software en un proceso continuo, predecible y seguro. Muchas gracias."*
