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