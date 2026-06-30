# BAT_BIBLE.md

**Documento:** BAT Bible
**Versión:** 2.0.0
**Estado:** Activo
**Compatible con:** BAT v1.4.x+

---

# 1. Propósito

La BAT Bible define las reglas oficiales para el desarrollo de BOARDING AGENT TOOLS (BAT). Todo cambio funcional, técnico o arquitectónico deberá respetar este documento.

# 2. Visión

Convertir BAT en la plataforma de referencia para Boarding Agents mediante una aplicación confiable, rápida, modular y preparada para operar aun sin conexión a Internet.

# 3. Misión

Proporcionar herramientas digitales que simplifiquen las operaciones portuarias, reduzcan errores operativos y centralicen el conocimiento del Boarding Agent.

# 4. Principios

1. Offline First.
2. Compatibilidad hacia atrás.
3. JSON como fuente oficial de datos.
4. Interfaces simples y consistentes.
5. Código reutilizable antes que duplicado.
6. Documentación y código evolucionan juntos.
7. Cada versión debe ser estable antes de agregar nuevas funciones.

# 5. Arquitectura

- HTML
- CSS
- JavaScript
- Progressive Web App
- LocalStorage
- GitHub Pages
- Service Worker

# 6. Reglas de Desarrollo

- Analizar impacto antes de programar.
- Mantener compatibilidad.
- Evitar duplicar lógica.
- Preferir funciones reutilizables.
- Documentar decisiones relevantes.
- Mantener nombres claros y consistentes.

# 7. Reglas de UI

- Diseño uniforme.
- Navegación consistente.
- Botones con comportamiento predecible.
- Lenguaje claro.
- Optimizado para escritorio y móvil.

# 8. Versionado

Toda versión debe actualizar:

- version.json
- Service Worker (CACHE_NAME)
- Changelog
- Documentación

# 9. Flujo Oficial

Idea
→ Backlog
→ Análisis
→ Desarrollo
→ Pruebas
→ Documentación
→ Versionado
→ Publicación

# 10. Definición de Terminado

Un cambio sólo se considera terminado cuando:

- Código implementado.
- Probado.
- Documentación actualizada.
- Changelog actualizado.
- Decisión registrada (si aplica).
- Versión incrementada.
- Service Worker actualizado.
- BAT Patch generado.

# 11. Principios para IA

Toda IA que participe en BAT deberá:

- Leer START_HERE.md.
- Consultar esta BAT Bible.
- Mantener compatibilidad.
- No eliminar funcionalidades existentes sin una decisión documentada.
- Priorizar estabilidad sobre velocidad de desarrollo.

# 12. Anti‑Patterns

Nunca:

- Romper compatibilidad.
- Duplicar lógica.
- Publicar sin pruebas.
- Modificar la estructura JSON sin documentarlo.
- Omitir la actualización del CACHE_NAME cuando sea necesaria.

# 13. Architecture Decision Records (ADR)

ADR-0001: La documentación oficial reside en BAT-Documentation.

ADR-0002: BAT adopta una arquitectura Offline First.

ADR-0003: JSON es la fuente oficial de datos.

ADR-0004: La compatibilidad hacia atrás es obligatoria.

ADR-0005: Cada publicación debe mantener sincronizados código y documentación.

# 14. Frase Oficial

> "Cada línea de código debe hacer a BAT más estable, más simple y más útil para el Boarding Agent."

---
Historial

v2.0.0
- Primera edición de la BAT Bible para BAT-Documentation.
