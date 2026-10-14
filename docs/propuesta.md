# Propuesta Metodológica

## Propuesta de metodología para la elaboración del inventario de sistemas de IA en el Ayuntamiento de Málaga

---

## 1. Fase de Identificación

La primera fase de la elaboración del inventario consiste en identificar todos los sistemas de IA utilizados por la entidad. Esta fase es crítica: un sistema no identificado no puede clasificarse, evaluarse ni supervisarse.

Para garantizar la exhaustividad, se propone un enfoque híbrido que combina dos mecanismos complementarios: una encuesta descendente a todos los departamentos, y una revisión técnica ascendente de sistemas, contratos y proveedores.

### 1.1 Criterios de Inclusión: ¿Qué es un Sistema de IA?

Antes de iniciar la identificación, es necesario establecer una definición operativa de "sistema de IA". Se adopta la definición del Reglamento Europeo de IA (Artículo 3.1):

> Sistema basado en máquinas diseñado para funcionar con distintos niveles de autonomía, que puede mostrar capacidad de adaptación tras su despliegue, y que, para objetivos explícitos o implícitos, infiere de la información de entrada que recibe cómo generar resultados, como predicciones, contenidos, recomendaciones o decisiones, que pueden influir en entornos físicos o virtuales.

En términos prácticos, un sistema se incluye en el inventario si cumple los siguientes criterios:

- Utiliza técnicas de aprendizaje automático, aprendizaje profundo, lógica difusa, sistemas expertos, o modelos generativos.
- Genera predicciones, clasificaciones, recomendaciones, contenido o decisiones.
- Se utiliza en la actividad administrativa, la atención ciudadana, la gestión interna o la prestación de servicios públicos.

Se excluyen del inventario las herramientas ofimáticas sin componentes de IA, las bases de datos convencionales y los sistemas de automatización puramente basados en reglas fijas sin capacidad de inferencia.

### 1.2 Mecanismo 1: Encuesta Descendente a Departamentos

Se diseña un cuestionario estructurado que se distribuye a todos los departamentos municipales. El cuestionario debe ser comprensible para personal no técnico y debe permitir respuestas tanto afirmativas como negativas.

El cuestionario incluye las siguientes preguntas:

1. ¿Utiliza su departamento alguna herramienta o sistema que genere predicciones, clasificaciones, recomendaciones o contenido de forma automática?
2. ¿Utiliza su departamento herramientas de inteligencia artificial generativa (por ejemplo, asistentes de texto, generación de imágenes, análisis automatizado de documentos)?
3. ¿Ha contratado su departamento algún servicio o producto que incluya componentes de inteligencia artificial?
4. ¿Utiliza su departamento sistemas que analicen datos de la ciudadanía para tomar decisiones o priorizar actuaciones?
5. Si la respuesta a alguna de las preguntas anteriores es afirmativa, proporcione el nombre del sistema, el proveedor, el departamento responsable y una breve descripción de su uso.

Las respuestas se recopilan en un formulario único y se centralizan en la unidad responsable de la gobernanza de IA.

### 1.3 Mecanismo 2: Revisión Técnica Ascendente

En paralelo a la encuesta, se realiza una revisión técnica de los sistemas, contratos y proveedores de la entidad. Esta revisión permite identificar sistemas que los departamentos no hayan reconocido como IA, o que se hayan adquirido sin conocimiento centralizado.

La revisión comprende:

- **Revisión de contratos y licencias de software**: identificación de productos y servicios que incluyan componentes de IA.
- **Revisión de la cartera de aplicaciones**: análisis de los sistemas en producción para detectar funcionalidades de IA no declaradas.
- **Revisión de proveedores**: consulta a los principales proveedores tecnológicos sobre los componentes de IA incorporados en los productos contratados.
- **Revisión de proyectos en curso**: identificación de iniciativas de IA en fase de diseño o implementación.

### 1.4 Consolidación del Inventario Inicial

Los resultados de ambos mecanismos se consolidan en un inventario inicial. Para cada sistema identificado se registra la siguiente información mínima:

| Campo | Descripción |
|-------|-------------|
| Identificador | Código único del sistema |
| Nombre | Denominación del sistema |
| Departamento responsable | Unidad que utiliza el sistema |
| Proveedor | Entidad que lo proporciona, si es externo |
| Descripción funcional | Qué hace el sistema |
| Tipo de IA | Técnica utilizada (aprendizaje automático, generativa, etc.) |
| Datos tratados | Categorías de datos que procesa |
| Usuarios afectados | Personas o grupos sobre los que impacta |
| Estado | En producción, en desarrollo, en desuso |

El inventario inicial se somete a validación por parte de los departamentos, que confirman o corrigen la información registrada.

### 1.5 Conexión con la Fase de Clasificación

Una vez consolidado el inventario inicial, cada sistema se somete a la fase de clasificación según su nivel de riesgo, que se desarrolla en la sección siguiente.

## 2. Fase de Clasificación

Una vez consolidado el inventario inicial, cada sistema identificado se somete a un proceso de clasificación según su nivel de riesgo. Esta clasificación determina las obligaciones aplicables y el nivel de control que debe ejercer la entidad.

La clasificación no depende de la tecnología utilizada, sino del **uso** del sistema y de las personas afectadas por él. Se articula en cuatro preguntas sucesivas, que permiten detener el análisis en cuanto el nivel de riesgo queda determinado.

### 2.1 Primera Pregunta: ¿Cuál es la finalidad prevista del sistema?

La finalidad prevista es el uso para el que el sistema está destinado por su proveedor, incluyendo el contexto específico y las condiciones de uso. No es lo que el sistema podría hacer en teoría, sino lo que está diseñado para hacer en la práctica.

Esta información se obtiene del campo "descripción funcional" del inventario y, cuando sea necesario, de la documentación del proveedor.

Si la finalidad no puede determinarse con claridad, el sistema se marca como "requiere análisis adicional" y se solicita información complementaria al departamento responsable y al proveedor.

### 2.2 Segunda Pregunta: ¿Opera el sistema en un ámbito del Anexo III?

Se revisa si el sistema opera en alguno de los ámbitos de alto riesgo enumerados en el Anexo III del Reglamento Europeo de IA. Los ámbitos más relevantes para una entidad local son:

| Ámbito del Anexo III | Ejemplos en el contexto municipal |
|----------------------|-----------------------------------|
| Infraestructuras críticas | Gestión de tráfico, suministro de agua, gestión de emergencias |
| Educación y formación profesional | Evaluación de estudiantes, asignación de plazas |
| Empleo y gestión de trabajadores | Selección de personal, evaluación del desempeño |
| Acceso a servicios públicos esenciales | Evaluación de elegibilidad para ayudas, priorización de emergencias |
| Aplicación de la ley | Sistemas de vigilancia, identificación biométrica |
| Migración y asilo | Evaluación de solicitudes, control fronterizo |
| Administración de justicia | Asistencia en la toma de decisiones judiciales |
| Procesos democráticos | Sistemas que influyen en el voto o la participación política |

Si el sistema opera en uno de estos ámbitos, se presume de alto riesgo y se pasa a la tercera pregunta para confirmar o descartar la clasificación.

Si el sistema no opera en ninguno de estos ámbitos, se pasa directamente a la cuarta pregunta.

### 2.3 Tercera Pregunta: ¿Realiza el sistema elaboración de perfiles?

La elaboración de perfiles implica el tratamiento automatizado de datos personales para evaluar aspectos personales de una persona física, como su rendimiento, situación económica, salud, preferencias, intereses, fiabilidad o comportamiento.

Un sistema que realiza elaboración de perfiles se considera **siempre de alto riesgo**, con independencia del ámbito en que opere.

Esta pregunta es especialmente relevante para sistemas que cruzan múltiples conjuntos de datos para inferir características de las personas. Un ejemplo identificado en el análisis de Málaga es el uso de datos de padrón, catastro y urbanismo para identificar poblaciones vulnerables ante inundaciones. Este cruce de datos constituye una inferencia sobre circunstancias personales y, por tanto, una actividad de elaboración de perfiles.

Si el sistema realiza elaboración de perfiles, se clasifica como **alto riesgo** y finaliza el análisis.

Si el sistema no realiza elaboración de perfiles, se pasa a la cuarta pregunta.

### 2.4 Cuarta Pregunta: ¿Cuál es el papel del ser humano en la decisión?

Se examina si el sistema toma decisiones de forma autónoma o si apoya a un ser humano que toma la decisión final.

El Reglamento Europeo de IA establece que un sistema puede no considerarse de alto riesgo si realiza únicamente una tarea procedimental limitada, mejora el resultado de una actividad humana previa, o detecta patrones de decisión sin sustituir la evaluación humana.

Sin embargo, esta excepción no se aplica si el sistema realiza elaboración de perfiles de personas físicas.

Para evaluar el papel humano se analizan tres elementos:

- **¿Puede el operador revisar la información y la recomendación del sistema antes de actuar?**
- **¿Tiene el operador capacidad real de anular la recomendación?**
- **¿Existe constancia documental de las anulaciones y sus motivos?**

Si el ser humano revisa activamente y puede anular con criterio propio, el sistema puede clasificarse como de **riesgo limitado** (obligaciones de transparencia) o **riesgo mínimo**.

Si el ser humano se limita a confirmar de forma automática la salida del sistema, la decisión es funcionalmente automatizada y el sistema debe clasificarse como de **alto riesgo**.

### 2.5 Resultado de la Clasificación

El resultado de las cuatro preguntas se registra en el inventario mediante los siguientes campos:

| Campo | Valores posibles |
|-------|------------------|
| Ámbito del Anexo III aplicable | Ninguno / Infraestructuras críticas / Empleo / Servicios esenciales / Otros |
| ¿Realiza elaboración de perfiles? | Sí / No |
| Papel del ser humano | Revisión activa / Confirmación automática / Sin intervención humana |
| **Clasificación final** | **Riesgo inaceptable / Alto riesgo / Riesgo limitado / Riesgo mínimo** |
| Justificación | Explicación breve del razonamiento aplicado |

### 2.6 Obligaciones Derivadas de la Clasificación

La clasificación determina las obligaciones que la entidad debe cumplir:

| Clasificación | Obligaciones principales |
|---------------|--------------------------|
| Riesgo inaceptable | Prohibición de uso |
| Alto riesgo | Evaluación de conformidad, supervisión humana, transparencia, registro, evaluación de impacto |
| Riesgo limitado | Información al usuario sobre la interacción con IA |
| Riesgo mínimo | Sin obligaciones específicas, buenas prácticas recomendadas |

### 2.7 Conexión con la Fase de Evaluación

La clasificación no es un fin en sí mismo. Es el punto de partida para la fase de evaluación, en la que se analizan los riesgos específicos de cada sistema y se determinan las medidas de control necesarias. Esta fase se desarrolla en la sección siguiente.