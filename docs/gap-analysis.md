# Análisis de Brechas

## 1. Marco de Clasificación: El Artículo 6 del Reglamento Europeo de IA

El Reglamento Europeo de Inteligencia Artificial clasifica los sistemas según su nivel de riesgo, y la clasificación depende de la **finalidad prevista del sistema**, no de la tecnología que utilice. El artículo 6 del Reglamento (en su redacción vigente tras el Ómnibus digital sobre IA) establece dos vías de acceso a la condición de alto riesgo y un orden de análisis que conviene respetar:[^1]

1. **Artículo 6.1**: el sistema es componente de seguridad de un producto regulado en el Anexo I (maquinaria, dispositivos médicos, juguetes) y ese producto requiere evaluación de conformidad por terceros. Esta vía resulta poco frecuente en una administración local. Sus obligaciones se aplican desde el 2 de agosto de 2028.
2. **Artículo 6.2**: el sistema encaja en alguno de los ocho ámbitos del Anexo III (biometría, infraestructuras críticas, educación, empleo, acceso a servicios esenciales, aplicación de la ley, migración, justicia y procesos democráticos). Sus obligaciones se aplican desde el 2 de diciembre de 2027.
3. **Artículo 6.3**: un sistema del Anexo III puede no considerarse de alto riesgo si no plantea un riesgo importante para la salud, la seguridad o los derechos fundamentales y cumple alguna de cuatro condiciones (tarea procedimental limitada, mejora de una actividad humana previa, detección de patrones sin sustituir la valoración humana, tarea preparatoria). **Excepción decisiva**: esta vía de exclusión nunca está disponible si el sistema efectúa elaboración de perfiles de personas físicas. En ese caso, el sistema del Anexo III siempre será de alto riesgo. Cabe precisar el alcance de esta regla: se aplica a sistemas que ya están en el Anexo III. La elaboración de perfiles, por sí sola, no convierte en alto riesgo a un sistema que no encaja en el Anexo III, aunque seguirá estando sujeta al RGPD (artículos 4.4 y 22).[^2]
4. **Artículo 6.4**: el proveedor que acoja su sistema a la exclusión del 6.3 debe documentar su evaluación antes de ponerlo en servicio y registrar esa decisión en la base de datos de la UE. Es decir, incluso la conclusión de "no es de alto riesgo" exige un expediente documentado.
5. **Artículo 50**: los sistemas que interactúan con personas o generan contenido sintético tienen obligaciones de transparencia, en vigor desde el 2 de agosto de 2026. A esta categoría se acogen, por ejemplo, los asistentes de IA integrados en herramientas ofimáticas.

**Conclusión metodológica**: clasificar un sistema exige conocer su finalidad prevista, sus datos, sus usuarios y su contexto de uso. Sin esa información, el artículo 6 no puede aplicarse. La clasificación es, por tanto, la primera operación que un inventario debe posibilitar.

## 2. Clasificación Preliminar: GeDIA

Sobre la base de la documentación pública disponible (octubre de 2026), que describe a GeDIA como una plataforma de gemelo digital orientada a la planificación urbana, la predicción de necesidades de infraestructuras y el análisis del crecimiento poblacional y turístico:[^3]

| Campo | Evaluación |
| --- | --- |
| ¿Encaja en algún ámbito del Anexo III? | No de forma manifiesta en la finalidad documentada. La planificación y previsión urbanística no equivale, por sí sola, a ser componente de seguridad de una infraestructura crítica ni a priorizar emergencias o conceder prestaciones. |
| ¿Está en el ámbito de infraestructuras críticas del Anexo III? | Solo si el sistema se utiliza como componente de seguridad en la gestión operativa de infraestructuras (por ejemplo, gestión del tráfico o del suministro de agua). La documentación pública no permite afirmarlo ni descartarlo. |
| ¿Efectúa elaboración de perfiles de personas físicas? | No consta en la documentación pública. Si el sistema cruzara datos personales (padrón, catastro, registros municipales) para inferir aspectos personales (vulnerabilidad, situación económica), estaría efectuando elaboración de perfiles a efectos del RGPD. |
| **Clasificación con la información pública disponible** | **No determinable.** |

Esta indeterminación no es un fallo del análisis: es la demostración del problema. El artículo 6 exige conocer la finalidad prevista y el tratamiento de datos del sistema, y esa información no es pública para ninguno de los sistemas municipales conocidos. Una ficha de sistema completa, del tipo que propone este documento, permitiría resolver la clasificación en horas.

**Análisis condicional.** Si la verificación documental revelara que GeDIA se utiliza en la gestión operativa de emergencias (priorización de llamadas, despacho de recursos, identificación de poblaciones afectadas) o que cruza datos personales para evaluar circunstancias personales, el sistema entraría en el ámbito del Anexo III (acceso a servicios públicos esenciales, e infraestructuras críticas si aplica) y la vía de exclusión del 6.3 quedaría cerrada en caso de elaboración de perfiles. En ese escenario, la clasificación sería de alto riesgo, con las obligaciones correspondientes a partir del 2 de diciembre de 2027.

## 3. Clasificación Preliminar: Google Workspace con Gemini

| Campo | Evaluación |
| --- | --- |
| ¿Encaja la herramienta, como producto, en el Anexo III? | No. Es una suite de productividad de propósito general con un modelo de IA integrado. |
| ¿Pueden encajar usos concretos de la herramienta en el Anexo III? | Sí. Depende del uso que cada departamento haga de ella. Ejemplos potenciales: cribado de candidaturas en selección de personal (ámbito de empleo), evaluación automatizada del desempeño, o apoyo a decisiones sobre solicitudes de ayudas (ámbito de servicios esenciales). |
| ¿Aplica el artículo 50 (transparencia)? | Sí, en vigor desde el 2 de agosto de 2026. Las personas que interactúan con el asistente deben ser informadas de que interactúan con IA, salvo excepciones, y el contenido generado debe identificarse cuando sea pertinente. |
| ¿Aplica el RGPD? | Siempre que circulen datos personales por las herramientas, con las obligaciones habituales (base jurídica, minimización, EIPD cuando proceda). El uso de Gemini sobre datos de la ciudadanía o de empleados puede requerir evaluación de impacto. |
| **Clasificación preliminar** | **Requiere análisis por caso de uso.** La herramienta, como tal, no es de alto riesgo; algunos de sus usos departamentales podrían serlo. |

**Implicación práctica.** Con más de 3.500 usuarios, la probabilidad de que existan usos de alto riesgo entre los departamentos es elevada.[^4] La única forma de detectarlos es un registro de casos de uso: cada departamento que utilice capacidades de IA sobre datos de personas debería declarar qué hace, con qué datos y con qué efectos. Este registro puede integrarse en el inventario general propuesto en este documento, y su coste es marginal frente al riesgo de una clasificación errónea.

## 4. Brecha Identificada

El análisis anterior revela una brecha con tres capas:

- **Brecha de información**: no existe documentación pública (ni, a saber, interna verificable) que permita aplicar el artículo 6 a los sistemas conocidos. Ni siquiera la exclusión del 6.3, que exige documentar la evaluación, podría sustanciarse hoy.
- **Brecha de obligación**: la Declaración de Málaga compromete a las entidades a elaborar un inventario antes del próximo Congreso de RECI, y el calendario del Reglamento (transparencia ya en vigor, alto riesgo desde diciembre de 2027) convierte ese inventario en condición previa de cumplimiento.
- **Brecha metodológica**: ningún documento de referencia define cómo ejecutar la identificación, la clasificación y el registro de los sistemas. Esta última capa es la que aborda la propuesta de este documento.

---

## Fuentes

[^1]: Artículo 6 del Reglamento (UE) 2024/1689, en su redacción vigente. Texto consolidado disponible en el Servicio de asistencia del AI Act de la Comisión Europea: [https://ai-act-service-desk.ec.europa.eu/es/ai-act/article-6](https://ai-act-service-desk.ec.europa.eu/es/ai-act/article-6) y en EUR-Lex: [https://eur-lex.europa.eu/eli/reg/2024/1689/oj](https://eur-lex.europa.eu/eli/reg/2024/1689/oj)

[^2]: Reglamento (UE) 2016/679 (RGPD), artículo 4.4 (definición de elaboración de perfiles) y artículo 22 (decisiones individuales automatizadas). Texto consolidado disponible en: [https://eur-lex.europa.eu/eli/reg/2016/679/oj](https://eur-lex.europa.eu/eli/reg/2016/679/oj)

[^3]: Documentación pública del proyecto GeDIA (Grupo Cibernos). Disponible en: [https://www.grupocibernos.com/proyecto-gedia](https://www.grupocibernos.com/proyecto-gedia)

[^4]: Nota de prensa del Ayuntamiento de Málaga sobre Google Workspace con Gemini (18 de diciembre de 2025). Disponible en: [https://www.malaga.eu/el-ayuntamiento/notas-de-prensa/detalle-de-la-nota-de-prensa/index.html?id=177140](https://www.malaga.eu/el-ayuntamiento/notas-de-prensa/detalle-de-la-nota-de-prensa/index.html?id=177140)