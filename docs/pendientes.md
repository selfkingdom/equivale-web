# Errores conocidos y tareas pendientes

## EQ-001

**Alta · Abierto · Totales solapados en el histórico.** El apilado admite sumar un total y sus componentes, como recaudación tributaria total e IVA. Cierra al impedir que esas selecciones produzcan un total engañoso y verificar un caso con conceptos independientes. [Código](../index.html)

## EQ-002

**Alta · Cerrado · Despliegue.** El 27 de noviembre de 2026 se verificaron el proveedor, la rama y la versión servida. Consulta el [procedimiento y la evidencia](despliegue.md).

## EQ-003

**Media · Abierto · Acciones sobre un importe inválido.** El conversor vacía el resultado, pero el texto compartido puede contener `NaN`. Cierra al comprobar que las acciones requieren un resultado válido y funcionan al corregir la entrada. [Código](../index.html)

## EQ-004

**Media · Pendiente de verificar · Formulario de diagnóstico.** El archivo sigue en el repositorio y usa el destino de producción del formulario principal. Cierra al confirmar su exposición y decidir si sigue siendo necesario. [Formulario](../prueba-contacto.html)

## EQ-005

**Media · Abierto · Eventos pendientes al cambiar de día.** Sustituir la partida puede descartar su cola de estadísticas. Cierra al definir el comportamiento esperado y verificarlo con una transición de fecha sin conexión. [Código](../index.html)

## EQ-006

**Media · Abierto · Navegación con teclado en las pestañas.** Faltan vínculos accesibles con los paneles y manejo de flechas. Cierra al verificar navegación, foco y relaciones entre pestañas y paneles. [Código](../index.html)

## EQ-007

**Media · Abierto · Comprobaciones al actualizar datos.** El conversor, el histórico y el reto combinan datos compartidos con cifras específicas. Cierra al disponer de comprobaciones repetibles de fuentes, unidades y años, ajuste de IPC y coherencia de los ejemplos entre funciones. [Arquitectura](arquitectura.md)

## EQ-008

**Alta · Pendiente de verificar · Web Analytics en el dominio actual.** Comprueba en Cloudflare el hostname configurado, la disponibilidad del histórico anterior y la recepción de una visita de `equivale.net`. La documentación del proveedor permite editar el hostname de una instalación manual. El efecto sobre el histórico de esta propiedad está pendiente de comprobar en el panel. [Documentación de Cloudflare](https://developers.cloudflare.com/web-analytics/get-started/)

## EQ-009

**Media · Pendiente de verificar · Recepción de estadísticas de Adivina.** Verifica por separado la llegada de eventos consentidos desde el origen de producción al Worker y su registro. El cliente y la configuración del Worker tienen ciclos de despliegue independientes. [Arquitectura](arquitectura.md)
