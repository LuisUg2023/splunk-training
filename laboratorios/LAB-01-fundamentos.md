# LAB-01 — Reconocimiento de Splunk e inicio de búsquedas

**Etapa:** Fundamentos de Splunk  
**Estado:** Diseño documental; no registrar como laboratorio ejecutado.

## 1. Objetivo
Reconocer la interfaz de Splunk, identificar las áreas principales de búsqueda y explorar eventos de un conjunto de datos de práctica.

## 2. Alineación formativa
Etapa 1 de la ruta oficial: fundamentos e introducción a Splunk.

## 3. Requisitos
- Acceso autorizado a un entorno Splunk de práctica.
- Dataset de entrenamiento o datos sintéticos.
- Permisos para consultar el índice seleccionado.

## 4. Procedimiento propuesto
1. Iniciar sesión en el entorno autorizado.
2. Identificar la aplicación de búsqueda y los menús disponibles.
3. Revisar el selector de rango temporal.
4. Identificar índices y tipos de fuente disponibles.
5. Ejecutar una búsqueda general sobre un índice de práctica.
6. Revisar eventos, campos y metadatos.
7. Guardar la consulta y documentar lo observado.

## 5. Consultas iniciales ilustrativas
Reemplazar `<indice_practica>` por un índice existente:

```spl
index=<indice_practica> earliest=-24h
| head 20
```

Contar eventos por tipo de fuente:

```spl
index=<indice_practica> earliest=-24h
| stats count by sourcetype
| sort -count
```

## 6. Resultado esperado
Visualizar eventos disponibles y reconocer campos como `_time`, `host`, `source` y `sourcetype`, cuando estén presentes en el dataset.

## 7. Resultado observado
Completar después de ejecutar. No asumir que el índice, los eventos o los campos existen antes de verificarlos.

## 8. Evidencias
Agregar capturas reales de:
- Interfaz principal de búsqueda.
- Consulta ejecutada y rango temporal.
- Eventos y campos obtenidos.

Sanitizar usuarios, direcciones, nombres de host y cualquier dato sensible.

## 9. Análisis y conclusión
Completar con base en los resultados reales, indicando limitaciones del dataset y aprendizajes obtenidos.
