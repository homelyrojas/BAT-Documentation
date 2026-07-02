# Decision Log

Registrar únicamente decisiones importantes.

Formato:

Fecha Decisión Motivo Alternativas Resultado

Este documento representa la memoria arquitectónica del proyecto.

## 2026-07-02 | BAT Import Engine inicial

Decisión: Crear `bat-import.js` como motor reutilizable de importación para datos operativos copiados desde Excel, correo o texto plano.

Motivo: El parser de Próximos Buques dependía demasiado de tabulaciones perfectas o bloques rígidos de 7 campos. Eso provocaba que registros válidos se descartaran cuando había notas vacías, servicios `N/A`, espacios no separables o texto copiado desde correo.

Alternativas evaluadas:
- Parchear únicamente `proximos-buques.js`.
- Mantener el parser actual y documentar el formato exacto de captura.
- Crear un motor reutilizable para Próximos Buques y futuros módulos de Buques.

Resultado: Se adopta la tercera alternativa. `proximos-buques.js` queda como consumidor del motor y no como dueño de toda la lógica de importación. Esto reduce deuda técnica y prepara el camino para reutilizar el motor en Arribos y Zarpes, Schematic y futuros módulos.
