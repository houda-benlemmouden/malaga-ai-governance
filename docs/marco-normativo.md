# Marco Normativo

Esta sección recoge los marcos regulatorios y metodológicos aplicables al análisis de gobernanza de inteligencia artificial en el sector público, con su estado de vigencia a octubre de 2026. Se distingue en todo momento entre normas jurídicas obligatorias y marcos voluntarios de buenas prácticas.

---

## 1. Reglamento Europeo de Inteligencia Artificial

El Reglamento (UE) 2024/1689 establece un marco jurídico armonizado para el desarrollo, la comercialización y el uso de sistemas de inteligencia artificial en la Unión Europea. Su enfoque es basado en el riesgo: las obligaciones dependen del nivel de riesgo que el sistema representa para los derechos fundamentales y la seguridad de las personas.[^1]

### 1.1 Niveles de Riesgo y Calendario de Aplicación

Tras su modificación por el Reglamento (UE) 2026/1744 (Ómnibus digital sobre IA, en vigor desde el 27 de julio de 2026), el calendario de aplicación es el siguiente:[^2]

| Nivel | Descripción | Obligaciones | Aplicable desde |
| --- | --- | --- | --- |
| Riesgo inaceptable | Prácticas prohibidas por atentar contra derechos fundamentales | Prohibición total | 2 de febrero de 2025 |
| Alto riesgo (Anexo III) | Sistemas de los ocho ámbitos del Anexo III (biometría, infraestructuras críticas, educación, empleo, servicios esenciales, aplicación de la ley, migración, justicia y procesos democráticos) | Gestión de riesgos, evaluación de conformidad, supervisión humana, transparencia, registro en la base de datos de la UE | 2 de diciembre de 2027 |
| Alto riesgo (Anexo I) | Componentes de seguridad de productos regulados | Las anteriores, integradas en la evaluación de conformidad del producto | 2 de agosto de 2028 |
| Riesgo limitado | Sistemas con obligaciones de transparencia (chatbots, contenido sintético) | Informar al usuario de que interactúa con IA; identificar contenido generado | 2 de agosto de 2026 (en vigor) |
| Riesgo mínimo | Mayoría de los sistemas | Sin obligaciones específicas; códigos de conducta voluntarios |  |

### 1.2 Reglas de Clasificación (Artículo 6)

Un sistema es de alto riesgo por dos vías (artículos 6.1 y 6.2). La exclusión del 6.3 (tarea procedimental limitada, mejora de actividad humana previa, detección de patrones, tarea preparatoria) no está disponible cuando el sistema efectúa elaboración de perfiles de personas físicas, y en todo caso exige documentar la evaluación y registrarla (6.4). La elaboración de perfiles, por sí sola, no eleva a alto riesgo a un sistema que no encaje en el Anexo III, aunque activa obligaciones del RGPD.[^3] Véase el análisis detallado en la sección [Análisis de Brechas](gap-analysis.md).

### 1.3 Obligaciones ya en Vigor

A octubre de 2026 resultan ya exigibles: las prácticas prohibidas (desde febrero de 2025), las obligaciones de los modelos de IA de uso general (desde agosto de 2025) y las obligaciones de transparencia del artículo 50 (desde agosto de 2026). Además, los responsables del despliegue que sean autoridades públicas deberán registrar sus sistemas de alto riesgo en la base de datos de la UE (artículos 49 y 71) antes de la fecha de aplicación del Anexo III. La norma también mantiene, con formulación actualizada, el deber de adoptar medidas de apoyo a la alfabetización en IA del personal que utiliza estos sistemas (artículo 4).

---

## 2. Reglamento General de Protección de Datos y Normativa Española de Protección de Datos

El RGPD (Reglamento (UE) 2016/679) es aplicable a todo tratamiento de datos personales que realicen los sistemas de IA. Sus obligaciones relevantes incluyen:[^4]

- **Base jurídica del tratamiento**: todo tratamiento debe tener una base legal (artículo 6).
- **Limitación de la finalidad y minimización de datos**: los datos solo se utilizan para los fines previstos y en la medida necesaria.
- **Evaluación de Impacto relativa a la Protección de Datos (EIPD)**: obligatoria cuando el tratamiento entraña alto riesgo, en particular cuando se efectúa elaboración de perfiles a gran escala (artículo 35).
- **Decisiones automatizadas**: las personas tienen derecho a no ser objeto de decisiones basadas únicamente en tratamiento automatizado con efectos significativos, con excepciones (artículo 22).
- **Elaboración de perfiles**: definida en el artículo 4.4 como todo tratamiento automatizado de datos personales para evaluar aspectos personales.

En España, la Ley Orgánica 3/2018 (LOPDGDD) complementa al RGPD y regula aspectos específicos del tratamiento por las administraciones públicas, incluido el deber de designar un delegado de protección de datos (artículo 37 del RGPD y disposición adicional).[^5]

---

## 3. ISO/IEC 42001: Sistema de Gestión de IA

ISO/IEC 42001 (ISO/IEC 42001:2023) es el primer estándar internacional certificable que especifica requisitos para un Sistema de Gestión de Inteligencia Artificial (SGIA). Es un marco **voluntario**, sin fuerza de ley, pero certificable y cada vez más exigido en contratación pública tecnológica. Su estructura sigue el modelo armonizado de sistemas de gestión:[^6]

| Cláusula | Contenido |
| --- | --- |
| 4. Contexto de la organización | Comprensión del contexto, partes interesadas y alcance del SGIA |
| 5. Liderazgo | Compromiso de la dirección, política de IA, roles y responsabilidades |
| 6. Planificación | Riesgos y oportunidades, evaluación de riesgos de IA, objetivos |
| 7. Apoyo | Recursos, competencia, concienciación, comunicación, información documentada |
| 8. Operación | Planificación y control operacional, tratamiento de riesgos de IA |
| 9. Evaluación del desempeño | Seguimiento, medición, auditoría interna, revisión por la dirección |
| 10. Mejora | No conformidad, acción correctiva, mejora continua |

El Anexo A desarrolla controles en áreas como políticas, organización interna, recursos, evaluación de impacto de los sistemas, datos para IA, información a las partes interesadas, uso de sistemas de IA y relaciones con terceros. El inventario propuesto en este documento constituye, en términos del estándar, información documentada de apoyo a las cláusulas 6, 8 y 9.

---

## 4. NIST AI Risk Management Framework

El marco del NIST (AI RMF 1.0) es un marco **voluntario** de gestión de riesgos de IA, organizado en cuatro funciones:[^7]

| Función | Propósito |
| --- | --- |
| Govern (Gobernar) | Políticas, responsabilidades y cultura de gestión de riesgos |
| Map (Mapear) | Contexto, riesgos y partes interesadas |
| Measure (Medir) | Evaluación y monitorización de riesgos |
| Manage (Gestionar) | Priorización y tratamiento de riesgos |

El marco define siete características de la IA fiable: válida y fiable, segura, protegida y resiliente, responsable y transparente, explicable e interpretable, con privacidad mejorada, y justa con los sesgos perjudiciales gestionados. En julio de 2024 el NIST publicó además un perfil específico para riesgos de IA generativa (NIST AI 600-1), pertinente para herramientas como los asistentes integrados en suites de productividad.

---

## 5. Metodología FEMP.IA y Guía FEMP

La Federación Española de Municipios y Provincias (FEMP) publicó en diciembre de 2025 la Guía Práctica y Políticas de Uso de la Inteligencia Artificial en las Entidades Locales y su metodología de autoevaluación FEMP.IA, referencia adoptada por la Declaración de Málaga.[^8]

El modelo FEMP.IA estructura la evaluación en tres niveles de madurez: administración electrónica (AE), automatización robótica de procesos (RPA) e inteligencia artificial (IA). El formulario de autoevaluación para el nivel directivo se organiza en cinco bloques: estrategia, tecnología, talento y cultura, gobernanza y ética, y resultados y métricas.

---

## 6. Esquema Nacional de Seguridad

El Real Decreto 43/2021 regula el Esquema Nacional de Seguridad (ENS), de aplicación obligatoria a las administraciones públicas españolas en materia de seguridad de los sistemas de información, incluidos los que incorporan componentes de IA. El compromiso séptimo de la Declaración de Málaga (garantizar la ciberseguridad) se apoya directamente en este marco. La normativa de desarrollo del ENS (CCN-STIC) publica guías específicas sobre seguridad en sistemas de IA.[^9]

---

## 7. Estado de Vigencia (octubre de 2026)

| Marco | Naturaleza | Estado |
| --- | --- | --- |
| Reglamento (UE) 2024/1689, modificado por (UE) 2026/1744 | Norma europea, directamente aplicable | En vigor, aplicación escalonada (véase 1.1) |
| RGPD y LOPDGDD 3/2018 | Norma de protección de datos | En vigor |
| ENS (RD 43/2021) | Norma española de seguridad | En vigor |
| Proyecto de ley de buen uso y gobernanza de la IA | Norma española de desarrollo del AI Act | En tramitación parlamentaria (aprobado en Consejo de Ministros el 26/05/2026); designará a AESIA como autoridad de supervisión |
| ISO/IEC 42001:2023 | Estándar voluntario certificable | Publicado; en uso en contratación pública |
| NIST AI RMF 1.0 y perfil de IA generativa | Marco voluntario | Publicados |
| Guía FEMP y metodología FEMP.IA | Marco sectorial de referencia | Publicadas en diciembre de 2025 |

---

## 8. Referencias Cruzadas

Este marco sirve de base a las secciones [Análisis de Brechas](gap-analysis.md) y [Propuesta Metodológica](propuesta.md).

---

## Fuentes

[^1]: Reglamento (UE) 2024/1689. Texto consolidado disponible en EUR-Lex: [https://eur-lex.europa.eu/eli/reg/2024/1689/oj](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)

[^2]: Reglamento (UE) 2026/1744 (Ómnibus digital sobre IA), publicado en el DOUE el 24 de julio de 2026 y en vigor desde el 27 de julio de 2026. Disponible en: [https://eur-lex.europa.eu/legal-content/ES/TXT/?uri=CELEX:32026R1744](https://eur-lex.europa.eu/legal-content/ES/TXT/?uri=CELEX:32026R1744)

[^3]: Servicio de asistencia del AI Act de la Comisión Europea, texto consolidado del artículo 6: [https://ai-act-service-desk.ec.europa.eu/es/ai-act/article-6](https://ai-act-service-desk.ec.europa.eu/es/ai-act/article-6)

[^4]: Reglamento (UE) 2016/679 (RGPD). Texto consolidado disponible en: [https://eur-lex.europa.eu/eli/reg/2016/679/oj](https://eur-lex.europa.eu/eli/reg/2016/679/oj)

[^5]: Ley Orgánica 3/2018 (LOPDGDD). Disponible en: [https://www.boe.es/buscar/act.php?id=BOE-A-2018-16673](https://www.boe.es/buscar/act.php?id=BOE-A-2018-16673)

[^6]: ISO/IEC 42001:2023. Disponible en: [https://www.iso.org/standard/42001](https://www.iso.org/standard/42001)

[^7]: NIST AI Risk Management Framework 1.0 y NIST AI 600-1 (perfil de IA generativa). Disponibles en: [https://www.nist.gov/itl/ai-risk-management-framework](https://www.nist.gov/itl/ai-risk-management-framework)

[^8]: Guía Práctica y Políticas de Uso de la Inteligencia Artificial en las Entidades Locales y metodología FEMP.IA. Disponibles en: [https://www.femp.es](https://www.femp.es)

[^9]: Real Decreto 43/2021 (ENS). Disponible en: [https://www.boe.es/buscar/act.php?id=BOE-A-2021-1861](https://www.boe.es/buscar/act.php?id=BOE-A-2021-1861)