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

## 3. Fase de Validación y Mantenimiento

Un inventario no es un documento estático. Es un registro vivo que debe reflejar la realidad cambiante de los sistemas de IA en la organización. Esta fase garantiza que el inventario sea completo, preciso y esté actualizado.

### 3.1 Validación de la Exhaustividad

La validación tiene como objetivo confirmar que el inventario refleja todos los sistemas de IA en uso, no solo los declarados voluntariamente.

Se aplican tres mecanismos complementarios:

**Mecanismo 1: Contraste con la revisión técnica**

Los resultados de la encuesta se contrastan con los resultados de la revisión técnica de contratos, aplicaciones y proveedores. Si un sistema aparece en la revisión técnica pero no en la encuesta, se investiga la discrepancia y se incorpora al inventario.

**Mecanismo 2: Confirmación por los departamentos**

Cada departamento recibe el extracto del inventario que le corresponde y debe confirmar por escrito que la información es completa y correcta. Esta confirmación tiene dos efectos:

- Traslada la responsabilidad de la exhaustividad al departamento.
- Crea un registro documental de la declaración realizada.

La confirmación no es una formalidad. Es un acto con consecuencias. Si un sistema no declarado se identifica posteriormente, la entidad dispone de un registro que muestra qué departamento omitió la información y cuándo.

**Mecanismo 3: Revisión cruzada entre departamentos**

Determinados sistemas afectan a varios departamentos. Por ejemplo, un sistema de gestión de ayudas sociales puede ser utilizado por Servicios Sociales pero alimentado con datos de otros departamentos. La revisión cruzada permite identificar sistemas que ningún departamento considera propios pero que están en uso.

### 3.2 Gestión de Sistemas No Declarados

Cuando se identifica un sistema de IA que no fue declarado en la encuesta inicial, se activa el siguiente procedimiento:

1. **Registro del sistema** en el inventario con la marca de "identificado en validación".
2. **Notificación al departamento** correspondiente, solicitando información funcional y confirmación.
3. **Análisis de la causa** de la omisión: desconocimiento, adquisición descentralizada, cambio de proveedor, u otras causas.
4. **Incorporación al ciclo de clasificación** conforme a la sección 2.

Este procedimiento no tiene carácter sancionador. Su finalidad es corregir el inventario, no penalizar al departamento. No obstante, la reiteración de omisiones en un mismo departamento puede dar lugar a acciones de formación o de control interno.

### 3.3 Actualización Periódica

El inventario se actualiza conforme a tres ciclos:

| Ciclo | Frecuencia | Contenido |
|-------|------------|-----------|
| Ciclo ordinario | Trimestral | Incorporación de nuevos sistemas, actualización de estados, revisión de sistemas en desarrollo |
| Ciclo de revisión | Anual | Revisión completa del inventario, reclasificación de sistemas, actualización de evaluaciones |
| Ciclo extraordinario | Cuando ocurra | Incorporación de sistemas adquiridos de urgencia, cambios normativos, incidentes relevantes |

### 3.4 Integración con los Procesos de Contratación

Para evitar que nuevos sistemas de IA se incorporen sin conocimiento de la unidad de gobernanza, se establece la siguiente medida:

- **Criterio de inclusión en contratación**: todo contrato de adquisición de software o servicios tecnológicos debe incluir una declaración del proveedor sobre la presencia de componentes de IA.
- **Revisión previa**: la unidad de gobernanza de IA revisa los contratos que incluyan componentes de IA antes de su formalización.
- **Registro automático**: los sistemas identificados en contratación se incorporan al inventario desde su fase de diseño.

Esta integración convierte la contratación en una fuente sistemática de identificación, en lugar de depender exclusivamente de la declaración de los departamentos.

### 3.5 Conexión con la Autoevaluación FEMP.IA

El inventario es un insumo para la autoevaluación de madurez prevista en la metodología FEMP.IA. Los datos del inventario permiten responder a las preguntas del formulario de madurez directiva en los bloques de gobernanza, ética y resultados.

La autoevaluación, a su vez, identifica áreas de mejora que se incorporan al plan de mejora previsto en la Declaración de Málaga.

### 3.6 Conexión con la Fase de Evaluación

Una vez validado y actualizado el inventario, cada sistema de alto riesgo se somete a la fase de evaluación, en la que se analizan los riesgos específicos y se determinan las medidas de control necesarias. Esta fase se desarrolla en la sección siguiente.

## 4. Fase de Evaluación

La clasificación determina qué sistemas son de alto riesgo. La evaluación determina qué riesgos específicos presentan esos sistemas y qué medidas deben adoptarse para controlarlos.

Esta fase se aplica obligatoriamente a los sistemas clasificados como de **alto riesgo**. Para los sistemas de riesgo limitado y mínimo, se aplican medidas proporcionadas al nivel de riesgo identificado.

### 4.1 Dimensiones de la Evaluación

La evaluación analiza cada sistema de alto riesgo en seis dimensiones, alineadas con el Reglamento Europeo de IA, el RGPD y el marco NIST de gestión de riesgos de IA.

| Dimensión | Pregunta de evaluación |
|-----------|------------------------|
| **Supervisión humana** | ¿Puede un ser humano comprender, supervisar e intervenir en el funcionamiento del sistema? |
| **Transparencia y explicabilidad** | ¿Puede explicarse el funcionamiento del sistema a las personas afectadas y a los responsables de su supervisión? |
| **Protección de datos y privacidad** | ¿Trata el sistema datos personales? ¿Se ha realizado una Evaluación de Impacto relativa a la Protección de Datos? |
| **Equidad y sesgo** | ¿Existe riesgo de que el sistema produzca resultados discriminatorios para determinados grupos? |
| **Seguridad y robustez** | ¿Está el sistema protegido contra ataques, manipulación y fallos técnicos? |
| **Trazabilidad y registro** | ¿Genera el sistema registros suficientes para auditar sus decisiones y detectar incidentes? |

### 4.2 Supervisión Humana

Se evalúa si el sistema permite una supervisión humana efectiva conforme al Artículo 14 del Reglamento Europeo de IA. Los elementos a verificar son:

- **Comprensión**: el operador humano comprende las capacidades y limitaciones del sistema.
- **Vigilancia**: el operador puede detectar anomalías, disfunciones y resultados inesperados.
- **Intervención**: el operador puede anular, corregir o detener el sistema.
- **Documentación**: las intervenciones humanas quedan registradas.

Si el sistema no permite una supervisión efectiva, se considera una deficiencia crítica que debe subsanarse antes de su uso continuado.

### 4.3 Transparencia y Explicabilidad

Se evalúa la capacidad de explicar el funcionamiento del sistema y las decisiones que produce. Los elementos a verificar son:

- **Información al usuario**: las personas afectadas son informadas de que están interactuando con un sistema de IA.
- **Explicación de decisiones**: las personas afectadas pueden obtener una explicación comprensible de las decisiones que les afectan, conforme al RGPD.
- **Documentación técnica**: existe documentación sobre el diseño, el funcionamiento y las limitaciones del sistema.

### 4.4 Protección de Datos y Privacidad

Se evalúa el cumplimiento del RGPD en el tratamiento de datos personales. Los elementos a verificar son:

- **Base jurídica**: existe una base legal para el tratamiento.
- **Minimización**: se tratan únicamente los datos necesarios.
- **Limitación de finalidad**: los datos se utilizan solo para los fines previstos.
- **Evaluación de Impacto**: se ha realizado una EIPD cuando el tratamiento entraña alto riesgo.
- **Derechos de las personas**: se garantizan los derechos de acceso, rectificación, supresión y oposición.

La EIPD es obligatoria cuando el sistema realiza elaboración de perfiles o trata categorías especiales de datos.

### 4.5 Equidad y Sesgo

Se evalúa el riesgo de que el sistema produzca resultados discriminatorios. Los elementos a verificar son:

- **Representatividad de los datos**: los datos de entrenamiento representan a la población afectada.
- **Métricas de equidad**: se han medido los resultados del sistema por grupos demográficos.
- **Detección de sesgos**: existen mecanismos para detectar y corregir sesgos.
- **Revisión periódica**: se revisan los resultados de forma continua para detectar derivas.

### 4.6 Seguridad y Robustez

Se evalúa la resistencia del sistema frente a ataques y fallos. Los elementos a verificar son:

- **Protección técnica**: el sistema está protegido contra accesos no autorizados y manipulación.
- **Resistencia a errores**: el sistema se comporta de forma predecible ante datos anómalos.
- **Gestión de incidentes**: existe un procedimiento para detectar, registrar y responder a incidentes.
- **Actualizaciones**: el sistema se mantiene actualizado conforme a las recomendaciones del proveedor.

### 4.7 Trazabilidad y Registro

Se evalúa la capacidad de auditar el funcionamiento del sistema. Los elementos a verificar son:

- **Registro automático**: el sistema genera registros de sus operaciones.
- **Conservación**: los registros se conservan durante el período exigido por la normativa.
- **Accesibilidad**: los registros están disponibles para auditoría interna y externa.
- **Reconstrucción**: es posible reconstruir una decisión concreta a partir de los registros.

### 4.8 Matriz de Evaluación

El resultado de la evaluación se registra en una matriz que refleja, para cada sistema y cada dimensión, el nivel de cumplimiento y las medidas pendientes.

| Dimensión | Nivel de cumplimiento | Medidas pendientes | Plazo | Responsable |
|-----------|-----------------------|--------------------|-------|-------------|
| Supervisión humana | Alto / Medio / Bajo | | | |
| Transparencia y explicabilidad | Alto / Medio / Bajo | | | |
| Protección de datos y privacidad | Alto / Medio / Bajo | | | |
| Equidad y sesgo | Alto / Medio / Bajo | | | |
| Seguridad y robustez | Alto / Medio / Bajo | | | |
| Trazabilidad y registro | Alto / Medio / Bajo | | | |

Los niveles de cumplimiento "Bajo" identifican deficiencias críticas que requieren actuación inmediata.

### 4.9 Plan de Medidas

Para cada deficiencia identificada se define una medida correctora con los siguientes elementos:

- **Descripción** de la medida.
- **Responsable** de su implementación.
- **Plazo** de ejecución.
- **Indicador** de cumplimiento.
- **Fecha de verificación**.

El plan de medidas se revisa periódicamente y se actualiza conforme se implementan las acciones.

### 4.10 Conexión con la Fase de Monitorización

La evaluación no es un ejercicio único. Una vez completada, los sistemas de alto riesgo se incorporan a un régimen de monitorización continua, en el que se revisan periódicamente los indicadores de riesgo y se actualizan las evaluaciones conforme evolucionan los sistemas y su contexto de uso.