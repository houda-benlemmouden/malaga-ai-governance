# Sobre Este Proyecto

## Autoría

Este documento ha sido elaborado por **Houda Benlemmouden**, profesional orientada a la gobernanza de la inteligencia artificial en el sector público.

El proyecto es en sí mismo la credencial principal: un análisis completo de gobernanza de IA aplicado a un caso real y reciente, construido desde cero sobre fuentes públicas, con metodología propia y verificación documental de cada afirmación de hecho. Antecedentes profesionales: soporte técnico de sistemas empresariales, análisis y documentación de programas de transformación digital y desarrollo de software, con formación complementaria en inteligencia artificial, automatización y marcos regulatorios europeos de IA.

Contacto:

- **LinkedIn**: [www.linkedin.com/in/houdab86](https://www.linkedin.com/in/houdab86)
- **Correo electrónico**: [houdaben3005@gmail.com](mailto:houdaben3005@gmail.com)
- **Repositorio**: [https://github.com/houda-benlemmouden/malaga-ai-governance](https://github.com/houda-benlemmouden/malaga-ai-governance)

## Motivación

La Declaración de Málaga, presentada el 16 de septiembre de 2026, establece once compromisos para el uso responsable de la inteligencia artificial en las ciudades. Entre sus medidas concretas, compromete a las entidades a elaborar un primer inventario accesible de los sistemas de IA utilizados antes del próximo Congreso de RECI y a realizar una autoevaluación de madurez mediante la metodología FEMP.IA.

Ni la Declaración ni los documentos de referencia que cita desarrollan, sin embargo, una metodología operativa para construir ese inventario. Este documento pretende contribuir a cubrir esa brecha, con una propuesta alineada con el Reglamento Europeo de IA (en su redacción vigente tras el Ómnibus digital sobre IA), el RGPD, la LOPDGDD, el Esquema Nacional de Seguridad, la norma ISO/IEC 42001, el marco NIST de gestión de riesgos de IA y la metodología FEMP.IA.

Este proyecto no tiene carácter oficial ni vinculación con el Ayuntamiento de Málaga, con RECI o con ninguna otra entidad mencionada. Se trata de un ejercicio profesional independiente de análisis y propuesta metodológica.

## Estructura del Documento

1. **[Estado Actual](current-state.md)**: el compromiso institucional de la Declaración de Málaga y los sistemas de IA con documentación pública disponible en la ciudad.
2. **[Análisis de Brechas](gap-analysis.md)**: aplicación del artículo 6 del Reglamento Europeo de IA a los sistemas conocidos y formulación de la brecha en tres capas (de información, de obligación y metodológica).
3. **[Marco Normativo](marco-normativo.md)**: los marcos jurídicos obligatorios y los marcos voluntarios aplicables, con su estado de vigencia a octubre de 2026.
4. **[Propuesta Metodológica](propuesta.md)**: metodología de inventario en cinco fases (identificación, clasificación, validación y mantenimiento, evaluación y monitorización), con entregables y plan de despliegue.

## Metodología de Trabajo

La información utilizada procede exclusivamente de fuentes públicas: la Declaración de Málaga, las notas de prensa institucionales del Ayuntamiento de Málaga, la documentación pública de los sistemas y proyectos citados y los textos oficiales de los marcos normativos. No se ha utilizado información confidencial ni datos internos de ninguna entidad.

Cada página incluye su lista de fuentes. Las afirmaciones que no han podido verificarse en fuentes públicas se han eliminado o se han reformulado como "aspectos no documentados públicamente", y el análisis jurídico se presenta de forma condicional cuando depende de hechos no verificables. La fecha de referencia de la verificación es el 16 de octubre de 2026.

## Limitaciones

- La clasificación de riesgo de los sistemas municipales no puede completarse desde fuentes públicas; es precisamente una de las conclusiones del documento.
- El proyecto de ley española de gobernanza de la IA está en tramitación parlamentaria; su aprobación podrá alterar aspectos del marco estatal descrito aquí.
- La propuesta metodológica no ha sido pilotada en un entorno real; las duraciones del plan de despliegue son orientativas.

## Resumen en Inglés (English Abstract)

This document analyzes the operational gap between the commitments of the Málaga Declaration on responsible AI (September 2026) and the absence of a published methodology for building the AI systems inventory the Declaration requires. Based solely on public sources, it applies Article 6 of the EU AI Act (as amended by the 2026 Digital Omnibus) to Málaga's publicly documented AI systems and proposes a five-phase inventory methodology (identification, classification, validation, evaluation, monitoring) aligned with the FEMP.IA maturity model, with a deployment plan sized for a local administration.

## Licencia y Reutilización

El contenido de este documento se publica bajo licencia Creative Commons BY 4.0: se permite su reproducción y adaptación con fines no comerciales citando a la autora. Las fichas, cuestionarios y plantillas derivados de la metodología pueden reutilizarse libremente por administraciones públicas.

## Aviso

Este documento se publica con fines de análisis y divulgación. Su contenido no constituye asesoramiento jurídico ni sustituye la consulta con profesionales especializados en la materia.

Este análisis refleja el estado de la información pública disponible a 16 de octubre de 2026. No se actualiza de forma continua. Las afirmaciones de hecho se basan en las fuentes citadas en cada página.

---

## Fuentes Principales

- **Declaración de Málaga** (VI Congreso Smart City RECI, 16 de septiembre de 2026): [https://www.malaga.eu/visorcontenido/ANUDocumentDisplayer/180023/COMUNICADO.pdf](https://www.malaga.eu/visorcontenido/ANUDocumentDisplayer/180023/COMUNICADO.pdf)
- **Nota de prensa del Ayuntamiento de Málaga** sobre la migración a Google Workspace con Gemini (18 de diciembre de 2025): [https://www.malaga.eu/el-ayuntamiento/notas-de-prensa/detalle-de-la-nota-de-prensa/index.html?id=177140](https://www.malaga.eu/el-ayuntamiento/notas-de-prensa/detalle-de-la-nota-de-prensa/index.html?id=177140)
- **Información corporativa de INNOVASUR** sobre el proyecto: [https://www.innovasur.com/](https://www.innovasur.com/)
- **Documentación pública del proyecto GeDIA** (Grupo Cibernos): [https://www.grupocibernos.com/proyecto-gedia](https://www.grupocibernos.com/proyecto-gedia)
- **Nota de prensa del Ayuntamiento de Málaga y Red.es** sobre el proyecto Centesimal (19 de marzo de 2026): [https://www.malaga.eu/visorcontenido/ANUDocumentDisplayer/179130/COMUNICADO.pdf](https://www.malaga.eu/visorcontenido/ANUDocumentDisplayer/179130/COMUNICADO.pdf)
- **Guía Práctica y Políticas de Uso de la Inteligencia Artificial en las Entidades Locales** (FEMP) y metodología FEMP.IA: [https://www.femp.es](https://www.femp.es)
- **Reglamento (UE) 2024/1689** (Reglamento Europeo de IA): [https://eur-lex.europa.eu/eli/reg/2024/1689/oj](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)
- **Reglamento (UE) 2026/1744** (Ómnibus digital sobre IA): [https://eur-lex.europa.eu/legal-content/ES/TXT/?uri=CELEX:32026R1744](https://eur-lex.europa.eu/legal-content/ES/TXT/?uri=CELEX:32026R1744)
- **Reglamento (UE) 2016/679** (RGPD) y **Ley Orgánica 3/2018** (LOPDGDD)
- **Real Decreto 43/2021** (Esquema Nacional de Seguridad)
- **ISO/IEC 42001:2023**: [https://www.iso.org/standard/42001](https://www.iso.org/standard/42001)
- **NIST AI Risk Management Framework**: [https://www.nist.gov/itl/ai-risk-management-framework](https://www.nist.gov/itl/ai-risk-management-framework)
- **Real Decreto 729/2023** (creación de AESIA)