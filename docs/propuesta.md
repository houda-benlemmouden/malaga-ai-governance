# Propuesta Metodológica

Propuesta de metodología para la elaboración del inventario de sistemas de IA en el Ayuntamiento de Málaga

---

La metodología se organiza en cinco fases: identificación, clasificación, validación y mantenimiento, evaluación y monitorización. Cada fase produce entregables concretos y se articula con la autoevaluación FEMP.IA prevista en la Declaración de Málaga. Al final de esta sección se incluye un plan de despliegue con duraciones orientativas.

## 1. Fase de Identificación

La primera fase consiste en identificar todos los sistemas de IA utilizados por la entidad. Es crítica: un sistema no identificado no puede clasificarse, evaluarse ni supervisarse.

Se propone un enfoque híbrido que combina dos mecanismos complementarios: una encuesta descendente a todos los departamentos y una revisión técnica ascendente de sistemas, contratos y proveedores.

### 1.1 Criterios de Inclusión: ¿Qué es un Sistema de IA?

Se adopta como definición operativa la del artículo 3.1 del Reglamento Europeo de IA:[^1]

> Sistema basado en máquinas diseñado para funcionar con distintos niveles de autonomía, que puede mostrar capacidad de adaptación tras su despliegue, y que, para objetivos explícitos o implícitos, infiere de la información de entrada que recibe cómo generar resultados, como predicciones, contenidos, recomendaciones o decisiones, que pueden influir en entornos físicos o virtuales.

En términos prácticos, un sistema se incluye en el inventario si cumple estos criterios:

- Utiliza técnicas de aprendizaje automático, aprendizaje profundo, lógica difusa, sistemas expertos o modelos generativos.
- Genera predicciones, clasificaciones, recomendaciones, contenido o decisiones.
- Se utiliza en la actividad administrativa, la atención ciudadana, la gestión interna o la prestación de servicios públicos.

Se excluyen las herramientas ofimáticas sin componentes de IA, las bases de datos convencionales y los sistemas de automatización basados en reglas fijas sin capacidad de inferencia. Los sistemas de IA integrados en herramientas de propósito general (por ejemplo, asistentes en suites ofimáticas) se incluyen, pero su clasificación se realiza por caso de uso (véase 2.5).

### 1.2 Mecanismo 1: Encuesta Descendente a Departamentos

Cuestionario estructurado distribuido a todos los departamentos, comprensible para personal no técnico:

1. ¿Utiliza su departamento alguna herramienta o sistema que genere predicciones, clasificaciones, recomendaciones o contenido de forma automática?
2. ¿Utiliza su departamento herramientas de inteligencia artificial generativa (asistentes de texto, generación de imágenes, análisis automatizado de documentos)?
3. ¿Ha contratado su departamento algún servicio o producto que incluya componentes de inteligencia artificial?
4. ¿Utiliza su departamento sistemas que analicen datos de la ciudadanía para tomar decisiones o priorizar actuaciones?
5. Si la respuesta a alguna pregunta anterior es afirmativa: nombre del sistema, proveedor, departamento responsable y breve descripción del uso.

Las respuestas se centralizan en la unidad responsable de la gobernanza de IA.

**Entregable**: formulario normalizado de identificación, reutilizable en cada ciclo de actualización.

### 1.3 Mecanismo 2: Revisión Técnica Ascendente

Revisión en paralelo de los sistemas, contratos y proveedores, para detectar sistemas no reconocidos como IA o adquiridos de forma descentralizada:

- Revisión de contratos y licencias de software.
- Revisión de la cartera de aplicaciones en producción.
- Consulta a los principales proveedores tecnológicos sobre componentes de IA incorporados en los productos contratados.
- Identificación de proyectos de IA en fase de diseño o implementación.

### 1.4 Consolidación del Inventario Inicial

Información mínima por sistema:

| Campo | Descripción |
| --- | --- |
| Identificador | Código único del sistema |
| Nombre | Denominación del sistema |
| Departamento responsable | Unidad que utiliza el sistema |
| Proveedor | Entidad que lo proporciona, si es externo |
| Descripción funcional | Qué hace el sistema y para qué se usa |
| Tipo de IA | Técnica utilizada (aprendizaje automático, generativa, etc.) |
| Datos tratados | Categorías de datos que procesa |
| Usuarios afectados | Personas o grupos sobre los que impacta |
| Estado | En producción, en desarrollo, en desuso |

El inventario inicial se valida por los departamentos, que confirman o corrigen la información registrada.

**Entregable**: registro maestro del inventario (hoja de cálculo o base de datos simple, sin coste de licencias).

## 2. Fase de Clasificación

Cada sistema se clasifica conforme al artículo 6 del Reglamento Europeo de IA, en el orden que el propio Reglamento sugiere. La clasificación determina las obligaciones aplicables y el nivel de control.[^2]

### 2.1 Primera Pregunta: ¿Cuál es la finalidad prevista del sistema?

La finalidad prevista es el uso para el que el sistema está destinado, con su contexto y condiciones de uso. Se obtiene del campo de descripción funcional y, cuando sea necesario, de la documentación del proveedor. Si no puede determinarse con claridad, el sistema se marca como "requiere análisis adicional" y se solicita información al departamento y al proveedor.

### 2.2 Segunda Pregunta: ¿Opera el sistema en un ámbito del Anexo III?

Se comprueba si el sistema encaja en alguno de los ocho ámbitos del Anexo III. Los más relevantes para una entidad local:

| Ámbito del Anexo III | Ejemplos en el contexto municipal |
| --- | --- |
| Infraestructuras críticas | Componente de seguridad en gestión de tráfico, suministro de agua o emergencias |
| Educación | Evaluación de estudiantes, asignación de plazas |
| Empleo | Selección de personal, evaluación del desempeño |
| Servicios públicos esenciales | Elegibilidad para ayudas, priorización de emergencias |
| Aplicación de la ley | Vigilancia, identificación biométrica |
| Procesos democráticos | Sistemas que influyen en participación política |

Si no encaja, se pasa a la pregunta 2.4. Si encaja, se presume alto riesgo y se aplica la siguiente comprobación.

### 2.3 Tercera Pregunta: ¿Puede excluirse el alto riesgo (artículo 6.3)?

El artículo 6.3 permite no considerar de alto riesgo a un sistema del Anexo III si no plantea riesgo importante y cumple alguna condición: tarea procedimental limitada, mejora del resultado de una actividad humana previa, detección de patrones sin sustituir la valoración humana, o tarea preparatoria.[^3]

**La exclusión nunca está disponible si el sistema efectúa elaboración de perfiles de personas físicas.** Tampoco para los sistemas del punto 2 del Anexo III (infraestructuras críticas) ni para los de clasificación y despacho de llamadas de emergencia (puntos 4.b y 4.c).

Si la exclusión resulta aplicable, el proveedor debe documentar su evaluación y registrarla (artículo 6.4), y esa documentación forma parte de la ficha del sistema. Si no resulta aplicable, el sistema se clasifica como **alto riesgo**.

Importante: la elaboración de perfiles no convierte por sí sola en alto riesgo a un sistema que no está en el Anexo III. En ese caso, sus efectos se canalizan por el RGPD (EIPD, artículo 22), pero la clasificación del sistema seguirá otro nivel.[^4]

### 2.4 Cuarta Pregunta: ¿Aplica el artículo 50 (transparencia)?

Los sistemas que no son de alto riesgo pero que interactúan con personas (chatbots, asistentes) o generan contenido sintético tienen obligaciones de transparencia en vigor desde el 2 de agosto de 2026: informar a la persona de que interactúa con IA e identificar el contenido generado cuando proceda.[^5] Estos sistemas se clasifican como de **riesgo limitado**. El resto, como de **riesgo mínimo**.

### 2.5 Sistemas de Propósito General: Clasificación por Caso de Uso

Las herramientas de propósito general con IA integrada (suites ofimáticas con asistentes, por ejemplo) se registran una vez en el inventario como plataforma y, además, cada departamento declara sus casos de uso con datos de personas. Un mismo asistente puede ser de riesgo mínimo en un uso (redacción interna) y de alto riesgo en otro (apoyo a la valoración de solicitudes de ayudas). Esta ficha de caso de uso es el mecanismo que convierte la clasificación de estas plataformas en algo operativo.

### 2.6 Registro del Resultado

| Campo | Valores posibles |
| --- | --- |
| Ámbito del Anexo III aplicable | Ninguno / Infraestructuras críticas / Empleo / Servicios esenciales / Otros |
| Exclusión del 6.3 aplicable | Sí / No / No evaluable (falta información) |
| ¿Realiza elaboración de perfiles? | Sí / No / No consta |
| Obligaciones de transparencia (art. 50) | Sí / No |
| **Clasificación final** | Alto riesgo / Riesgo limitado / Riesgo mínimo / Pendiente |
| Justificación | Explicación breve del razonamiento aplicado |

### 2.7 Obligaciones Derivadas y Calendario

| Clasificación | Obligaciones principales | Plazo |
| --- | --- | --- |
| Riesgo inaceptable | Cese del uso | Inmediato |
| Alto riesgo | Gestión de riesgos, documentación, supervisión humana, EIPD, registro en base de datos UE | 2 de diciembre de 2027 |
| Riesgo limitado | Información al usuario sobre la interacción con IA | En vigor (desde 2 de agosto de 2026) |
| Riesgo mínimo | Buenas prácticas y códigos de conducta voluntarios |  |

La evaluación de impacto en protección de datos no depende del calendario del AI Act: es obligatoria ya hoy cuando el tratamiento entraña alto riesgo (artículo 35 del RGPD).[^4]

## 3. Fase de Validación y Mantenimiento

Un inventario es un registro vivo. Esta fase garantiza que sea completo, preciso y actualizado.

### 3.1 Validación de la Exhaustividad

**Mecanismo 1: Contraste entre encuesta y revisión técnica.** Un sistema presente en la revisión técnica pero ausente de la encuesta se investiga y se incorpora.

**Mecanismo 2: Confirmación escrita por los departamentos.** Cada departamento confirma por escrito el extracto que le corresponde. Esto traslada la responsabilidad de la exhaustividad y crea un registro documental de la declaración.

**Mecanismo 3: Revisión cruzada entre departamentos.** Ciertos sistemas afectan a varias unidades; la revisión cruzada detecta sistemas que ningún departamento considera propio.

### 3.2 Gestión de Sistemas No Declarados

1. Registro del sistema con la marca "identificado en validación".
2. Notificación al departamento, con solicitud de información funcional.
3. Análisis de la causa de la omisión (desconocimiento, adquisición descentralizada, cambio de proveedor).
4. Incorporación al ciclo de clasificación.

El procedimiento no es sancionador. Su finalidad es corregir el inventario. La reiteración de omisiones en un mismo departamento puede dar lugar a acciones de formación o de control interno.

### 3.3 Actualización Periódica

| Ciclo | Frecuencia | Contenido |
| --- | --- | --- |
| Ordinario | Trimestral | Nuevos sistemas, estados, proyectos en desarrollo |
| Revisión | Anual | Revisión completa, reclasificaciones, actualización de evaluaciones |
| Extraordinario | Cuando ocurra | Adquisiciones urgentes, cambios normativos, incidentes relevantes |

### 3.4 Integración con la Contratación

- Todo contrato de software o servicios tecnológicos incluirá una declaración del proveedor sobre la presencia de componentes de IA.
- La unidad de gobernanza revisa los contratos con componentes de IA antes de su formalización.
- Los sistemas identificados se incorporan al inventario desde su fase de diseño.

### 3.5 Conexión con la Autoevaluación FEMP.IA

Los datos del inventario alimentan el formulario de madurez directiva (bloques de gobernanza, ética y resultados), y la autoevaluación devuelve áreas de mejora al plan previsto en la Declaración.

## 4. Fase de Evaluación

La clasificación determina qué sistemas son de alto riesgo. La evaluación determina qué riesgos específicos presentan y qué medidas se requieren. Se aplica a los sistemas clasificados como de alto riesgo antes del 2 de diciembre de 2027 y, de forma proporcionada, a los demás.

### 4.1 Dimensiones de la Evaluación

Seis dimensiones, alineadas con el Reglamento Europeo de IA, el RGPD y el marco NIST:

| Dimensión | Pregunta de evaluación |
| --- | --- |
| Supervisión humana | ¿Puede un ser humano comprender, supervisar e intervenir en el sistema? |
| Transparencia y explicabilidad | ¿Puede explicarse su funcionamiento a las personas afectadas y a los responsables? |
| Protección de datos y privacidad | ¿Trata datos personales? ¿Se ha realizado EIPD? |
| Equidad y sesgo | ¿Existe riesgo de resultados discriminatorios? |
| Seguridad y robustez | ¿Está protegido contra ataques, manipulación y fallos? |
| Trazabilidad y registro | ¿Genera registros suficientes para auditar sus decisiones? |

### 4.2 a 4.7: Guías de Evaluación por Dimensión

**Supervisión humana** (artículo 14 del Reglamento): el operador comprende las capacidades y limitaciones del sistema, puede detectar anomalías, puede anular o detenerlo, y sus intervenciones quedan registradas. Si el sistema no permite supervisión efectiva, la deficiencia es crítica y debe subsanarse antes de continuar su uso.

**Transparencia y explicabilidad**: las personas afectadas son informadas de que interactúan con IA (artículo 50, ya exigible); las decisiones automatizadas con efectos significativos tienen garantías del artículo 22 del RGPD; existe documentación técnica del sistema.

**Protección de datos**: base jurídica, minimización, limitación de finalidad, EIPD cuando proceda y garantía de los derechos de las personas. La EIPD es obligatoria ya hoy si el tratamiento entraña alto riesgo, con independencia del calendario del AI Act.

**Equidad y sesgo**: representatividad de los datos, métricas por grupos, mecanismos de detección y corrección de sesgos, revisión periódica.

**Seguridad y robustez**: protección técnica conforme al ENS, comportamiento predecible ante datos anómalos, procedimiento de gestión de incidentes, actualización según el proveedor.

**Trazabilidad**: registros automáticos de operaciones, conservación conforme a la normativa de archivo, disponibilidad para auditoría, capacidad de reconstruir decisiones concretas.

### 4.8 Matriz de Evaluación

| Dimensión | Nivel de cumplimiento | Medidas pendientes | Plazo | Responsable |
| --- | --- | --- | --- | --- |
| Supervisión humana | Alto / Medio / Bajo |  |  |  |
| Transparencia y explicabilidad | Alto / Medio / Bajo |  |  |  |
| Protección de datos y privacidad | Alto / Medio / Bajo |  |  |  |
| Equidad y sesgo | Alto / Medio / Bajo |  |  |  |
| Seguridad y robustez | Alto / Medio / Bajo |  |  |  |
| Trazabilidad y registro | Alto / Medio / Bajo |  |  |  |

Los niveles "Bajo" identifican deficiencias críticas que requieren actuación inmediata.

### 4.9 Plan de Medidas

Por cada deficiencia: descripción de la medida, responsable, plazo, indicador de cumplimiento y fecha de verificación. El plan se revisa periódicamente.

## 5. Fase de Monitorización

La evaluación ofrece una imagen en un momento determinado. Los sistemas, sus datos y su contexto cambian, y con ellos su nivel de riesgo.

### 5.1 Objetivos

Detectar derivas del comportamiento del sistema, detectar incidentes, verificar la eficacia de las medidas correctoras y mantener actualizada la clasificación.

### 5.2 Indicadores

| Categoría | Indicadores |
| --- | --- |
| Rendimiento | Precisión, tasa de falsos positivos y negativos |
| Equidad | Diferencias de resultados entre grupos, sesgos emergentes |
| Supervisión humana | Intervenciones y anulaciones registradas, con motivos |
| Incidentes | Número, tiempo de respuesta, resolución |

Cada indicador tiene un umbral de alerta que activa la revisión correspondiente.

### 5.3 Ciclos

| Ciclo | Frecuencia | Contenido |
| --- | --- | --- |
| Operativo | Mensual | Rendimiento e incidentes |
| Supervisión | Trimestral | Equidad y supervisión humana |
| Evaluación | Anual | Revisión completa y reclasificación |

### 5.4 Procedimiento ante Incidentes

1. Registro del incidente (qué ocurrió, sistema afectado, personas afectadas, impacto).
2. Evaluación inicial de gravedad y necesidad de medidas inmediatas.
3. Notificación a los órganos competentes y, cuando proceda, a la autoridad de supervisión.
4. Análisis de causa.
5. Medidas correctoras.
6. Verificación de su eficacia.

### 5.5 Actualización del Inventario

Los cambios de uso, de datos o de funciones pueden alterar la clasificación; cuando ocurren, el sistema vuelve a la fase 2. Los resultados de la monitorización alimentan, además, la autoevaluación FEMP.IA y cierran el ciclo de mejora continua.

## 6. Plan de Despliegue

Duraciones orientativas para un primer ciclo completo, asumible por una unidad pequeña:

| Fase | Duración estimada | Entregable principal |
| --- | --- | --- |
| 1. Identificación | 6 a 8 semanas | Registro maestro del inventario |
| 2. Clasificación | 4 a 6 semanas (parcialmente en paralelo) | Fichas de clasificación por sistema |
| 3. Validación | 2 a 4 semanas | Inventario validado con confirmaciones departamentales |
| 4. Evaluación | Proporcional al número de sistemas de alto riesgo (primera pasada antes del 2 de diciembre de 2027) | Matrices de evaluación y plan de medidas |
| 5. Monitorización | Continua a partir de la fase 4 | Informes periódicos de indicadores |

Con este calendario, el Ayuntamiento podría presentar un primer inventario validado en el próximo Congreso de RECI, cumpliendo el compromiso de la Declaración de Málaga, y dispondría de más de un año de margen para completar las evaluaciones antes de la entrada en vigor de las obligaciones de alto riesgo.

---

## Fuentes

[^1]: Reglamento (UE) 2024/1689, artículo 3.1 (definición de sistema de IA). Texto consolidado disponible en EUR-Lex: [https://eur-lex.europa.eu/eli/reg/2024/1689/oj](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)

[^2]: Reglamento (UE) 2024/1689, artículo 6 (reglas de clasificación). Texto consolidado disponible en el Servicio de asistencia del AI Act de la Comisión Europea: [https://ai-act-service-desk.ec.europa.eu/es/ai-act/article-6](https://ai-act-service-desk.ec.europa.eu/es/ai-act/article-6)

[^3]: Reglamento (UE) 2024/1689, artículo 6.3 y 6.4 (exclusiones y documentación). Disponible en: [https://eur-lex.europa.eu/eli/reg/2024/1689/oj](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)

[^4]: Reglamento (UE) 2016/679 (RGPD), artículos 4.4 (elaboración de perfiles), 22 (decisiones automatizadas) y 35 (EIPD). Texto consolidado disponible en: [https://eur-lex.europa.eu/eli/reg/2016/679/oj](https://eur-lex.europa.eu/eli/reg/2016/679/oj)

[^5]: Reglamento (UE) 2024/1689, artículo 50 (obligaciones de transparencia), aplicable desde el 2 de agosto de 2026. Disponible en: [https://eur-lex.europa.eu/eli/reg/2024/1689/oj](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)