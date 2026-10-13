# Marco Normativo

Esta sección recoge los marcos regulatorios y metodológicos aplicables al análisis de gobernanza de inteligencia artificial en el sector público.

---

## 1. Reglamento Europeo de Inteligencia Artificial

El Reglamento (UE) 2024/1689 establece un marco jurídico armonizado para el desarrollo, la comercialización y el uso de sistemas de inteligencia artificial en la Unión Europea. Su enfoque es **basado en el riesgo**: las obligaciones aplicables dependen del nivel de riesgo que el sistema representa para los derechos fundamentales y la seguridad de las personas.

### 1.1 Niveles de Riesgo

| Nivel | Descripción | Obligaciones |
|-------|-------------|--------------|
| **Riesgo inaceptable** | Prácticas prohibidas por atentar contra derechos fundamentales | Prohibición total |
| **Alto riesgo** | Sistemas incluidos en el Anexo III o que actúan como componentes de seguridad de productos regulados | Obligaciones estrictas: evaluación de conformidad, supervisión humana, transparencia, registro |
| **Riesgo limitado** | Sistemas con obligaciones de transparencia (por ejemplo, chatbots) | Informar al usuario de que interactúa con IA |
| **Riesgo mínimo** | Mayoría de sistemas | Sin obligaciones específicas |

### 1.2 Anexo III: Ámbitos de Alto Riesgo Relevantes

Dos ámbitos del Anexo III son directamente relevantes para el sector público local:

- **Infraestructuras críticas**: sistemas de IA utilizados como componentes de seguridad en la gestión de infraestructuras digitales críticas, tráfico rodado, o suministro de agua, gas, calefacción o electricidad.
- **Acceso a servicios públicos esenciales**: sistemas de IA utilizados para evaluar la elegibilidad de personas para servicios de asistencia pública esencial, o para la clasificación, despacho y priorización de llamadas de emergencia.

### 1.3 Elaboración de Perfiles (Profiling)

El Reglamento establece que un sistema de IA que realice **elaboración de perfiles** de personas físicas se considera siempre de alto riesgo. La elaboración de perfiles implica el tratamiento automatizado de datos personales para evaluar aspectos personales, como el rendimiento, la situación económica, la salud, las preferencias o la fiabilidad.

---

## 2. Reglamento General de Protección de Datos (RGPD)

El RGPD es aplicable a todo tratamiento de datos personales que realicen los sistemas de IA. Sus obligaciones relevantes incluyen:

- **Base jurídica del tratamiento**: todo tratamiento debe tener una base legal.
- **Limitación de la finalidad**: los datos solo pueden utilizarse para los fines para los que fueron recogidos.
- **Minimización de datos**: solo deben tratarse los datos necesarios.
- **Evaluación de Impacto relativa a la Protección de Datos (EIPD)**: obligatoria cuando el tratamiento entraña un alto riesgo para los derechos y libertades de las personas, en particular cuando implica elaboración de perfiles.
- **Derecho a la explicación**: las personas tienen derecho a obtener una explicación sobre las decisiones automatizadas que les afecten.

---

## 3. ISO/IEC 42001: Sistema de Gestión de IA

ISO/IEC 42001 es el primer estándar internacional que especifica los requisitos para establecer, implementar, mantener y mejorar un **Sistema de Gestión de Inteligencia Artificial (SGIA)**. Su estructura sigue el modelo armonizado de otros estándares de sistemas de gestión (como ISO 27001).

### 3.1 Estructura Principal

| Cláusula | Contenido |
|----------|-----------|
| 4. Contexto de la organización | Comprensión del contexto, partes interesadas y alcance del SGIA |
| 5. Liderazgo | Compromiso de la dirección, política de IA, roles y responsabilidades |
| 6. Planificación | Riesgos y oportunidades, evaluación de riesgos de IA, objetivos |
| 7. Apoyo | Recursos, competencia, concienciación, comunicación, información documentada |
| 8. Operación | Planificación y control operacional, tratamiento de riesgos de IA |
| 9. Evaluación del desempeño | Seguimiento, medición, auditoría interna, revisión por la dirección |
| 10. Mejora | No conformidad, acción correctiva, mejora continua |

### 3.2 Controles del Anexo A

Los controles del Anexo A se organizan en categorías como: ciclo de vida del sistema de IA, datos para sistemas de IA, información para las partes interesadas, uso de sistemas de IA, y relaciones con terceros y clientes.

---

## 4. NIST AI Risk Management Framework

El marco del NIST (Instituto Nacional de Estándares y Tecnología de Estados Unidos) proporciona una metodología para la gestión de riesgos de IA. Se organiza en cuatro funciones:

| Función | Propósito |
|---------|-----------|
| **Govern (Gobernar)** | Establecer políticas, responsabilidades y cultura de gestión de riesgos |
| **Map (Mapear)** | Identificar el contexto, los riesgos y las partes interesadas |
| **Measure (Medir)** | Evaluar y monitorizar los riesgos identificados |
| **Manage (Gestionar)** | Priorizar y tratar los riesgos |

El marco también define siete características de la IA fiable: válida y fiable, segura, protegida y resiliente, responsable y transparente, explicable e interpretable, con privacidad mejorada, y justa con sesgos perjudiciales gestionados.

---

## 5. Metodología FEMP.IA

La Federación Española de Municipios y Provincias (FEMP) ha desarrollado una guía práctica y una metodología de autoevaluación de madurez en IA para entidades locales. Esta metodología es la referencia adoptada por la Declaración de Málaga.

### 5.1 Modelo de Madurez

El modelo FEMP.IA estructura la evaluación en tres niveles:

- **Administración electrónica (AE)**
- **Automatización robótica de procesos (RPA)**
- **Inteligencia Artificial (IA)**

### 5.2 Formulario de Madurez Directiva

El formulario de autoevaluación para el nivel directivo se organiza en cinco bloques:

- Estrategia
- Tecnología
- Talento y cultura
- Gobernanza y ética
- Resultados y métricas

---

## 6. Referencias Cruzadas

Este marco normativo sirve de base para las secciones de [Análisis de Brechas](gap-analysis.md) y [Propuesta Metodológica](propuesta.md).