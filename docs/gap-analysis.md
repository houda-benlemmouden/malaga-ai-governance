## 5. Análisis de Brechas: Clasificación Preliminar de Sistemas

### 5.1 Metodología de Clasificación

El Reglamento Europeo de Inteligencia Artificial establece un enfoque basado en el riesgo. La clasificación no depende de la tecnología utilizada, sino del **uso** que se hace del sistema. Un sistema de IA se considera de alto riesgo cuando se utiliza en los ámbitos enumerados en el Anexo III del Reglamento.

Dos de estos ámbitos son directamente relevantes para el Ayuntamiento de Málaga:

- **Infraestructuras críticas**: sistemas de IA utilizados como componentes de seguridad en la gestión de infraestructuras digitales críticas, tráfico rodado, o suministro de agua, gas, calefacción o electricidad.
- **Acceso a servicios públicos esenciales**: sistemas de IA utilizados para evaluar la elegibilidad de personas para servicios de asistencia pública esencial, o para la **clasificación, despacho y priorización de llamadas de emergencia**.

Adicionalmente, el Reglamento establece que un sistema de IA que realice **elaboración de perfiles (profiling)** de personas físicas se considera siempre de alto riesgo.

### 5.2 Clasificación Preliminar: GeDIA

| Campo | Evaluación |
|-------|------------|
| **Área del Anexo III (si aplica)** | Acceso a servicios públicos esenciales — clasificación y priorización en emergencias |
| **¿Realiza elaboración de perfiles?** | Sí. El sistema cruza datos de padrón, catastro (IBI) y urbanismo para identificar poblaciones vulnerables, lo que constituye una inferencia sobre circunstancias personales. |
| **¿Es componente de seguridad de infraestructura crítica?** | Sí. El sistema se utiliza operativamente en coordinación con el Centro Municipal de Emergencias (CME) durante situaciones de emergencia por inundaciones. |
| **Clasificación preliminar** | **Alto riesgo** |
| **Justificación** | El sistema se utiliza para identificar y priorizar poblaciones vulnerables durante emergencias, lo que puede afectar el acceso a asistencia y protección. Además, realiza elaboración de perfiles mediante el cruce de múltiples conjuntos de datos personales. |

### 5.3 Clasificación Preliminar: Google Workspace con Gemini

| Campo | Evaluación |
|-------|------------|
| **Área del Anexo III (si aplica)** | No determinada. Depende del uso que cada departamento haga de la herramienta. |
| **¿Realiza elaboración de perfiles?** | No de forma inherente. El sistema es de propósito general. |
| **¿Es componente de seguridad de infraestructura crítica?** | No. Es una herramienta de productividad. |
| **Clasificación preliminar** | **Requiere análisis adicional** |
| **Justificación** | Al tratarse de un sistema de propósito general desplegado a más de 3.500 empleados, su clasificación depende del uso concreto. Algunos usos podrían ser de alto riesgo (por ejemplo, si se utiliza para evaluar solicitudes de ayuda social), mientras que otros serían de riesgo mínimo. La clasificación debe realizarse a nivel de caso de uso, no de herramienta. |

### 5.4 Brecha Identificada

El análisis anterior revela una brecha operativa significativa:

- La Declaración de Málaga compromete a las entidades a elaborar un inventario de sistemas de IA.
- El Reglamento Europeo de IA exige que los sistemas de alto riesgo cumplan obligaciones específicas.
- Sin embargo, **no existe una metodología definida** para identificar los sistemas de IA en uso, clasificarlos según su nivel de riesgo, y documentarlos en un registro accesible.

Esta brecha es el objeto de la propuesta que se presenta en la siguiente sección.