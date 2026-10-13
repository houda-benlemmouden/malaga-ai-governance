# Estado Actual de la Gobernanza de IA en Málaga

## 1. El Compromiso Institucional: La Declaración de Málaga

La Declaración de Málaga fue presentada el 16 de septiembre de 2026 en el marco del VI Congreso Smart City de la Red Española de Ciudades Inteligentes (RECI), celebrado en FYCMA (Palacio de Ferias y Congresos de Málaga). El documento fue entregado por Alicia Izquierdo, concejala delegada de Innovación, Digitalización y Captación de Inversiones del Ayuntamiento de Málaga, a Javier Peña, coordinador general de RECI, para que la Red lo incorpore como instrumento propio y le dé continuidad.

La Declaración establece once compromisos para avanzar hacia una incorporación responsable de la inteligencia artificial a la gestión municipal. Estos compromisos son:

1. Orientar el uso de la IA al interés general
2. Proteger los derechos de la ciudadanía
3. Garantizar la transparencia
4. Asumir la responsabilidad pública
5. Establecer la supervisión humana de los sistemas
6. Proteger la calidad de los datos
7. Garantizar la ciberseguridad
8. Realizar contratación tecnológica con garantías
9. Formar a los equipos municipales
10. Fomentar la cooperación entre ciudades
11. Asegurar la sostenibilidad ambiental de las soluciones de IA

El documento toma como referencia la Guía Práctica y Políticas de Uso de la Inteligencia Artificial en las Entidades Locales de la FEMP (Federación Española de Municipios y Provincias) y su metodología FEMP.IA.

## 2. Medidas Concretas de Evaluación y Seguimiento

La Declaración no se limita a principios. Establece medidas concretas para evaluar su aplicación:

- **Inventario de sistemas de IA**: Antes del próximo Congreso, cada entidad debe elaborar un primer inventario accesible de los sistemas de inteligencia artificial utilizados.
- **Autoevaluación de madurez**: Cada entidad debe realizar una autoevaluación de madurez mediante la metodología FEMP.IA, a partir de la cual se definirá un plan de mejora.
- **Revisión compartida**: Está prevista una revisión compartida a los seis meses.
- **Balance en el VII Congreso**: Se presentará un balance de la aplicación de la Declaración en el VII Congreso de RECI.

El Libro de Adhesiones a la Declaración de Málaga queda abierto a las ciudades de la Red y a otras entidades locales que compartan sus principios.

## 3. Estado de la Cuestión: La Brecha Operativa

La Declaración compromete a las entidades a elaborar un inventario de sistemas de IA y a realizar una autoevaluación de madurez. Sin embargo, ninguno de los documentos de referencia —ni la Declaración ni la Guía FEMP— proporciona una metodología estructurada para construir dicho inventario.

Específicamente, no se define:

- Cómo identificar los sistemas de IA en uso en los distintos departamentos municipales
- Cómo clasificar cada sistema según los niveles de riesgo del Reglamento Europeo de IA
- Cómo documentar los sistemas en un registro accesible y comprensible
- Cómo conectar el inventario con la autoevaluación de madurez FEMP.IA

Esta brecha operativa es el objeto del presente documento. El objetivo es proponer una metodología para la elaboración del inventario de sistemas de IA, alineada con el Reglamento Europeo de IA y con la metodología FEMP.IA, que permita a las entidades locales cumplir con los compromisos adquiridos en la Declaración de Málaga.

## 4. Sistemas de IA Desplegados en Málaga

### 4.1 GeDIA — Gemelo Digital de Ciudad

**¿Qué es?**
GeDIA es un gemelo digital de la ciudad de Málaga, una réplica virtual del entorno urbano que integra datos en tiempo real para simular escenarios y apoyar la toma de decisiones municipales. El sistema se utiliza operativamente en coordinación con el Centro Municipal de Emergencias (CME).

**¿Qué hace?**
El sistema utiliza redes neuronales LSTM, simulaciones de Monte Carlo y modelado basado en agentes para predecir el comportamiento de fenómenos como inundaciones. Durante la emergencia por lluvias de noviembre y diciembre de 2025, el Ayuntamiento utilizó la plataforma para:

- Simular escenarios de crecida de agua
- Identificar zonas potencialmente afectadas
- Detectar poblaciones vulnerables
- Localizar centros de evacuación

**¿Qué datos procesa?**
El sistema integra datos de más de 1.200 sensores IoT distribuidos en más de 200 ubicaciones (proyecto CENTESIMAL). Además, cruza datos de:

- Urbanismo
- Padrón municipal
- Catastro (IBI)

Esta integración de datos permite identificar poblaciones vulnerables ante inundaciones.

**¿Quién lo supervisa?**
El sistema se utiliza en coordinación con el Centro Municipal de Emergencias (CME). La responsabilidad política recae en el área de Innovación, Digitalización y Captación de Inversiones del Ayuntamiento de Málaga.

### 4.2 Google Workspace con Gemini

**¿Qué es?**
Es una migración de más de 3.500 puestos de trabajo municipales a Google Workspace con capacidades de inteligencia artificial mediante Gemini. La inversión asciende a 1,68 millones de euros.

**¿Qué hace?**
Proporciona a los empleados municipales herramientas de IA para:

- Creación de contenido
- Búsqueda y análisis de información
- Análisis de datos
- Procesamiento digital mediante formularios en línea y autenticación mejorada

**¿Qué datos procesa?**
El sistema procesa datos de los empleados municipales y potencialmente datos ciudadanos que circulan por las herramientas de Workspace. La naturaleza de estos datos depende del uso que cada departamento haga de las herramientas.

**¿Quién lo supervisa?**
La implementación está a cargo de INNOVASUR, socio tecnológico certificado en ISO 42001 (sistema de gestión de IA). La migración comenzó en 2025 y se espera completar en 2026.

### 4.3 Observación sobre el Inventario

Los dos sistemas documentados arriba representan únicamente los casos públicamente conocidos. No existe, a la fecha de este documento, un registro público accesible que enumere la totalidad de los sistemas de IA utilizados por el Ayuntamiento de Málaga. Esta ausencia es precisamente lo que la Declaración de Málaga se compromete a corregir antes del próximo Congreso de RECI.

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