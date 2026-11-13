# Comandos SPL fundamentales

Esta guía reúne los comandos trabajados como base de búsqueda y análisis en la ruta de Splunk Training. Los ejemplos son ilustrativos y requieren índices, sourcetypes y campos existentes en el entorno donde se ejecuten.

## Estructura básica
```spl
index=<indice> sourcetype=<tipo_de_fuente> earliest=-24h
```
- `index`: limita la búsqueda al índice indicado.
- `sourcetype`: filtra por formato o tipo de fuente.
- `earliest=-24h`: establece el inicio del rango temporal.

## Comandos principales

| Comando | Función | Ejemplo |
|---|---|---|
| `stats` | Calcula estadísticas agregadas. | `| stats count by status` |
| `sort` | Ordena los resultados. | `| sort -count` |
| `top` | Muestra los valores más frecuentes. | `| top limit=20 src_ip` |
| `timechart` | Agrega valores a lo largo del tiempo. | `| timechart count by sourcetype` |

## Ejemplos de análisis

### 1. Conteo de errores HTTP
```spl
index=web sourcetype=access_combined earliest=-24h status>=400
| stats count by status, clientip
| sort -count
```
Uso: agrupar respuestas HTTP de error por código y dirección de cliente.

### 2. Intentos de autenticación fallidos
```spl
index=security sourcetype=linux_secure earliest=-24h "failed password"
| top limit=20 src_ip
```
Uso: identificar las direcciones de origen más frecuentes en los eventos que coincidan con el texto.

### 3. Tendencia temporal de eventos
```spl
index=security earliest=-24h
| timechart count by sourcetype
```
Uso: observar la evolución temporal de eventos por tipo de fuente.

## Consideraciones
- Sustituir nombres de índices y campos por los existentes en el laboratorio.
- Verificar el rango temporal seleccionado.
- Revisar los eventos originales antes de interpretar una agregación.
- Documentar la consulta exacta y el resultado observado.
- Los resultados de ejemplo describen el propósito de la consulta; no son evidencia de ejecución.
