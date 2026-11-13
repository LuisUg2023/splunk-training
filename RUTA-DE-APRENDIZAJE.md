# Ruta de aprendizaje oficial — Splunk Training

> **Alcance:** esta ruta corresponde exclusivamente al catálogo y los recursos de Splunk Training. No incluye el curso «Introducción a Splunk» de Udemy ni el certificado de Google Cybersecurity de Coursera.

La secuencia está organizada por competencias y conserva los títulos de los cursos identificados en la plataforma. Las duraciones son las registradas durante la revisión del catálogo; pueden cambiar si Splunk actualiza sus contenidos.

## Etapa 1. Fundamentos de Splunk y operaciones de seguridad

| Curso oficial | Duración registrada | Contenido / competencia |
|---|---:|---|
| Intro to Splunk (eLearning) – Spanish Captions | 45 min | Introducción a Splunk, interfaz y conceptos iniciales. Estado registrado: Successful. |
| Security Operations and the Defense Analyst | 2 h | Operaciones de seguridad, funciones del analista y ciclo de trabajo defensivo. |
| The Cybersecurity Landscape | 3 h | Panorama de ciberseguridad, amenazas y contexto de defensa. |
| Introduction to Cybersecurity Awareness | 30 min | Fundamentos de concienciación y prácticas de seguridad. |
| Introduction to Splunk Security Essentials | 45 min | Casos de uso y contenido de seguridad en Splunk Security Essentials. |

**Temas transversales:** interfaz Search & Reporting, navegación, eventos, campos, índices, sourcetypes, hosts, fuentes de datos y flujo general de análisis.

**Práctica asociada:** LAB-01 — Reconocimiento de interfaz, fuentes de datos, eventos y búsquedas iniciales.

## Etapa 2. Búsqueda, SPL y análisis de datos

| Curso oficial | Duración registrada | Contenido / competencia |
|---|---:|---|
| Using Fields | 1 h | Identificación, selección y uso de campos. |
| Search Under the Hood | 1 h | Funcionamiento interno de las búsquedas y procesamiento de resultados. |
| Working with Time | 3 h | Rangos temporales, tiempo de búsqueda y análisis temporal. |
| Comparing Values | 3 h | Comparación de valores y condiciones en búsquedas. |
| Statistical Processing | 3 h | Procesamiento estadístico y agregaciones. |
| Result Modification | 3 h | Transformación, ordenamiento y modificación de resultados. |
| Creating Field Extractions | 3 h | Extracción y creación de campos. |
| Enriching Data with Lookups | 3 h | Enriquecimiento de eventos mediante tablas de búsqueda (lookups). |

**Temas SPL que deben quedar documentados y practicados:**
- Estructura de una búsqueda: índice, sourcetype, términos, filtros y rango temporal.
- Operadores booleanos AND, OR, NOT y agrupación de condiciones.
- Búsquedas por texto y frases exactas; diferencias entre buscar error, contraseña y la frase exacta "contraseña incorrecta".
- Campos y metadatos: _time, host, source, sourcetype y campos extraídos.
- Comparación y filtrado de valores.
- Comandos de transformación y análisis: stats, sort, top, timechart.
- Procesamiento de resultados, extracción de campos y lookup.
- Trabajos de búsqueda (search jobs), estado y tiempo de expiración de resultados.
- Interpretación de resultados y validación de la consulta frente a los eventos originales.

**Práctica asociada:** LAB-02 — Construcción, depuración e interpretación de consultas SPL.

## Etapa 3. Visualización, informes, alertas y objetos de conocimiento

| Curso oficial | Duración registrada | Contenido / competencia |
|---|---:|---|
| Visualizations | 1 h | Representación visual de resultados y selección de gráficos. |
| Creating Classic Dashboards | 2 h | Construcción de dashboards clásicos. |
| Scheduling Reports & Alerts | 3 h | Programación de informes y configuración de alertas. |
| Creating Knowledge Objects | 3 h | Creación y administración de objetos de conocimiento. |
| Data Models | 3 h | Organización y modelado de datos. |
| Introduction to Dashboards | 1 h | Introducción a dashboards y visualización de información. |

**Temas complementarios:**
- Aplicación Search & Reporting.
- Informes guardados y programados.
- Alertas, condiciones y acciones asociadas.
- Objetos de conocimiento y reutilización de búsquedas.
- Roles, permisos y acceso a búsquedas, informes y objetos.
- Modelos de datos y relación con el análisis de seguridad.
- Selección de visualizaciones según la pregunta analítica.

**Práctica asociada:** LAB-03 — Dashboard de monitoreo, informes programados y alertas.

## Etapa 4. Detección, análisis de amenazas y threat hunting

| Curso oficial | Duración registrada | Contenido / competencia |
|---|---:|---|
| Understanding Threats and Attacks | 4 h | Comprensión de amenazas, ataques y señales observables. |
| Introduction to Detection Engineering with Splunk | 2 h 30 min | Fundamentos de ingeniería de detección con Splunk. |
| SOC Essentials: Introduction to Threat Hunting | 4 h | Metodología inicial de búsqueda proactiva de amenazas. |
| Introduction to Enterprise Security | 40 min | Introducción a Splunk Enterprise Security. |
| Splunk Security Use Case Development: Using ESCU and Security Essentials | 4 h | Desarrollo de casos de uso de seguridad con ESCU y Security Essentials. |
| Using Splunk UBA | 4 h | Análisis de comportamiento de usuarios y entidades. |

**Competencias:** convertir hipótesis de amenaza en búsquedas, identificar patrones anómalos, comprender casos de uso, desarrollar detecciones y contextualizar alertas para un SOC.

**Práctica asociada:** LAB-04 — Detección de actividad sospechosa y documentación de una hipótesis de threat hunting.

## Etapa 5. Investigación y respuesta a incidentes

| Curso oficial | Duración registrada | Contenido / competencia |
|---|---:|---|
| The Art of Investigation | 6 h | Metodología de investigación y análisis de incidentes. |
| Introduction to Splunk SOAR | 20 min | Introducción a la automatización y orquestación de seguridad. |
| Implementing Splunk SOAR Community Playbooks | 30 min | Implementación de playbooks comunitarios. |
| Developing Splunk SOAR Apps | 3 h | Desarrollo de aplicaciones para Splunk SOAR. |
| Responding to Incidents in Splunk On-Call | 12 min | Gestión y respuesta a incidentes con Splunk On-Call. |

**Temas de trabajo:** reconstrucción cronológica de eventos, pivoteo entre campos y fuentes, documentación de hallazgos, priorización, playbooks, automatización y comunicación durante la respuesta.

**Práctica asociada:** LAB-05 — Investigación documentada de un incidente simulado y propuesta de respuesta.

## Etapa 6. Administración, operación y tecnologías de análisis

| Curso oficial | Duración registrada | Contenido / competencia |
|---|---:|---|
| Splunk Enterprise Installation and Configuration | 30 min | Instalación y configuración inicial de Splunk Enterprise. |
| Using the Monitoring Console | 30 min | Supervisión del estado y funcionamiento de Splunk. |
| Upgrading Splunk Enterprise | 17 min | Consideraciones para actualizar Splunk Enterprise. |
| Learning SPL2 Fundamentals | 2 h | Fundamentos del lenguaje SPL2. |
| Data and Tools for Defense Analysts | 6 h | Datos y herramientas para analistas de defensa. |

**Competencias:** comprender instalación y configuración, supervisión de la plataforma, mantenimiento y actualización, evolución de SPL hacia SPL2 y uso de datos/herramientas en actividades defensivas.

**Práctica asociada:** LAB-06 — Revisión de administración, monitoreo y operación en un entorno autorizado.

## Evaluaciones y ejercicios que forman parte del portafolio

Las evaluaciones ya trabajadas deben conservarse como registros independientes, sin mezclarlas con los laboratorios:

- **Banco de 15 preguntas técnicas:** conceptos de Splunk, operadores booleanos y búsquedas SPL, trabajos de búsqueda y expiración, Search & Reporting, roles y permisos, objetos de conocimiento e informes.
- **Evaluación 3 — Interpretación de búsquedas y análisis de resultados:** 10 preguntas; resultado registrado: 9 correctas y 1 incorrecta.
- **Evaluación 4 — Análisis integral de SPL en Splunk Enterprise:** evaluación de 10 preguntas en desarrollo. Se registró una respuesta inicial incorrecta al comparar búsquedas de errores HTTP con búsquedas de autenticación fallida. No registrar como aprobada ni completada.
- **Ejercicios SPL:** interpretación de consultas, operadores booleanos, filtros, comparación de términos, análisis estadístico y lectura crítica de resultados.

El detalle de estas actividades se documenta en [EVALUACIONES-Y-EJERCICIOS.md](./EVALUACIONES-Y-EJERCICIOS.md).

## Criterios de avance y evidencia

1. Mantener el título del curso como aparece en Splunk Training.
2. Registrar por separado estado, fecha, evaluación y evidencia de cada curso.
3. Diferenciar contenido revisado, ejercicio propuesto, ejercicio ejecutado y evaluación completada.
4. Añadir capturas reales de la plataforma, consultas y resultados cuando existan.
5. No atribuir resultados de laboratorio a consultas que no se hayan ejecutado.
6. No marcar como aprobado un curso o evaluación sin evidencia verificable.
7. Los laboratorios LAB-01 a LAB-06 son una estructura de práctica del portafolio; no equivalen a cursos oficiales ni se consideran completados por estar documentados.
