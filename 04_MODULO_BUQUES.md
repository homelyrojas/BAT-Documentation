# Módulos Buques

Incluye:
- Arribos y Zarpes
- Próximos Buques
- Schematic

Funciones:
- Bloque operativo
- Consulta por rango
- Solo MSC
- Consulta por nombre de buque
- Copiar resultados

Meta: Motor único de consultas operativas.

## Próximos Buques

### Estado v1.4.3

Se incorpora BAT Import Engine como primera pieza reutilizable para lectura de programación operativa pegada desde Excel, correo o texto tabulado.

### Campos esperados

- Buque
- Service
- ETA Fecha
- Hora
- Puerto de Arribo
- Puerto de Zarpe
- Notas

### Reglas de importación

- Acepta fechas en formato `d/m/yyyy`, `dd/mm/yyyy`, `d-m-yyyy` y `dd-mm-yyyy`.
- Acepta horas en formato `h:mm`, `hh:mm`, `h` y `hh`.
- Acepta notas vacías sin descartar el registro.
- Acepta servicio `N/A` para buques especiales o movimientos no asociados a servicio regular.
- Reconoce programación copiada desde Excel mediante tabulaciones.
- Reconoce programación pegada desde correos o texto plano cuando los campos se compactan por espacios.
- Elimina duplicados usando buque, ETA, hora, puerto de arribo y puerto de zarpe.

### Servicios reconocidos en v1.4.3

- CANADA GULF BRIDGE
- MEXICO GULF EXPRESS
- MEDGULF SERVICE
- PAMEX SERVICE
- N/A

### Puertos reconocidos en v1.4.3

- Altamira
- Veracruz
- Cristobal
- Cartagena
- Tampico
- Progreso
- Manzanillo
- Lázaro Cárdenas

### Archivos involucrados

- `bat-import.js`
- `proximos-buques.html`
- `proximos-buques.js`
- `service-worker.js`
- `version.json`

### Validación base

Con la programación de julio 2026 compartida por operación, el módulo debe procesar 15 buques:

- MSC NORDEROOG F
- MSC ALICANTE VI
- MSC ALDEBARAN III
- MSC JASPER VIII
- MSC NORDEROOG F
- MSC MAUREEN
- MSC AGAMEMNON VIII
- MSC KEY F
- HENRIKA SCHULTE
- MSC SAGITTA III
- MSC ARICA
- MSC NORDEROOG F
- MSC Phoenix
- MSC Damla
- MSC Magnum VII
