# Diario de desarrollo

## 2026-11-27 · Privacidad y analítica de la 5.15.0

- **Implementado:** apartado bilingüe de privacidad en el HTML local, reconstruido a partir del contenido descrito en el plan previo.
- **Probado:** sintaxis de JavaScript y ejecución de la localización del aviso en español e inglés. La comprobación de recepción de estadísticas queda en [EQ-008](pendientes.md#eq-008) y [EQ-009](pendientes.md#eq-009).
- **Aprobado:** Jorge revisó el aviso en local y autorizó publicar la versión en equivale.net y comprobar las estadísticas de Cloudflare.
- **Publicado:** pendiente. El panel de Cloudflare requiere inicio de sesión.

## 2026-11-27 · Verificación de producción

- **Implementado:** procedimiento de comprobación y reversión documentado. [EQ-002](pendientes.md#eq-002)
- **Probado:** consulta pública del HTML y comparación con el código local, más revisión de la ejecución de GitHub Pages. [Evidencia](despliegue.md)
- **Aprobado:** Jorge autorizó versionar la documentación y verificar producción. Se preparó una rama separada para la documentación.
- **Publicado:** se confirmó la versión de aplicación que ya estaba en producción. La verificación no inició un despliegue.

## 2026-11-27 · Sistema de documentación

- **Implementado:** estructura documental y reglas de mantenimiento en el árbol local. Consulta la [decisión 0001](decisiones/0001-documentacion-versionada.md).
- **Probado:** comprobación local de los archivos Markdown, su codificación, sus enlaces relativos y el alcance documental del cambio.
- **Aprobado:** Jorge aprobó la estructura y las reglas de mantenimiento antes de editar.
- **Publicado:** pendiente. El cambio está en el árbol local.

## 2026-11-27 · Auditoría inicial

Revisión de solo lectura del repositorio. La referencia de código y las comprobaciones constan en [Estado](estado.md). Los hallazgos que requieren seguimiento están en [Pendientes](pendientes.md).
