# Instrucciones de trabajo para Equivale

- Comunícate con Jorge y escribe la documentación del proyecto en español.
- Lee el [estado](docs/estado.md) y consulta la [arquitectura](docs/arquitectura.md) y los [pendientes](docs/pendientes.md) pertinentes. Comprueba el código y Git antes de dar por vigente un dato.
- Respeta el alcance autorizado. Distingue la edición local, el commit, el push y la publicación. Registra la autorización que corresponda a cada acción.
- El repositorio de GitHub es público. Mantén aquí contenido apto para publicación. Para futuras notas estratégicas privadas, usa solo una ubicación autorizada fuera del repositorio. Excluye credenciales y datos sensibles de la documentación y de los ejemplos.
- Usa Markdown UTF-8 y enlaces relativos estándar. Mantén estas instrucciones como fuente común para agentes. [CLAUDE.md](CLAUDE.md) importa este archivo.

## Cierre de una tarea significativa

Una tarea es significativa si cambia comportamiento, datos, arquitectura, integraciones, publicación, prioridades o procedimientos. Actualiza la documentación al cerrar la tarea, como parte del mismo trabajo y dentro del alcance autorizado.

1. Contrasta el resultado con el diff, el código, las pruebas ejecutadas y las comprobaciones externas que correspondan. Marca como pendiente cualquier dato que no se pueda verificar.
2. Actualiza las notas afectadas. El [estado](docs/estado.md) describe la situación vigente. La [arquitectura](docs/arquitectura.md) describe el funcionamiento. Los [pendientes](docs/pendientes.md) son el registro de tareas y errores. La [hoja de ruta](docs/hoja-de-ruta.md) enlaza esos identificadores. Las [decisiones](docs/decisiones/README.md) guardan el motivo de los cambios duraderos. El [historial](CHANGELOG.md) recoge los cambios que pertenecen a una versión.
3. Añade al [diario](docs/diario.md) una entrada breve con fecha, resultado, comprobaciones y enlaces a la evidencia o a las notas afectadas. Conserva cada detalle en su nota de referencia.
4. Comprueba los enlaces y revisa que cada afirmación coincide con la evidencia. Si el encargo es de solo lectura, comunica qué notas habría que actualizar y deja los archivos intactos.

## Estados de un cambio

Registra los cuatro estados por separado cuando sean pertinentes:

| Estado | Evidencia |
|---|---|
| Implementado | El cambio existe en el árbol local, en un commit o en un PR. Indica dónde. |
| Probado | Indica qué comprobaste, el resultado y qué quedó sin probar. |
| Aprobado | Cita la aprobación explícita y su alcance. |
| Publicado | Sigue el [procedimiento de despliegue](docs/despliegue.md) para verificar qué versión o commit sirve producción. Registra fecha y evidencia. Registra un push como un hecho distinto. |
