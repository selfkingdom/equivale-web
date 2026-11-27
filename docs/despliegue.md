# Despliegue y reversión

## Evidencia del 27 de noviembre de 2026

La [portada de Equivale](https://equivale.net/) respondió con HTTP 200 y cabecera `Server: GitHub.com`. El HTML declaró `5.14.0` y coincidió con el HTML de `163e4fe9fe3ed4dae5da9077f75740e8887467da` después de normalizar los saltos de línea a LF.

SHA-256 del HTML normalizado: `f3bcafd6e5dd71faf4cf2e19f0102be26c1c47c0438bd10550e834236255d4d2`.

La [ejecución de GitHub Pages](https://github.com/selfkingdom/equivale-web/actions/runs/45213664936) terminó correctamente para ese commit en `main`. La configuración de administración de Pages quedó fuera de la comprobación pública.

## Comprobar una publicación

1. Identifica el commit esperado. Revisa la rama, el SHA y el resultado en [GitHub Actions](https://github.com/selfkingdom/equivale-web/actions).
2. Descarga el HTML servido por HTTPS y lee la etiqueta `equivale-version`. Compara el contenido con el `index.html` del commit esperado, normalizando ambos a LF si corresponde.
3. Si el contenido difiere, comprueba el resultado de Pages y la caché antes de registrar la publicación. Documenta el resultado y la fecha en [Estado](estado.md) y, cuando corresponda, en el [historial](../CHANGELOG.md).

## Revertir una publicación

1. Identifica el cambio que se debe revertir y la última versión comprobada. Revisa el diff y los cambios posteriores que deban conservarse.
2. Prepara un commit de reversión en una rama y compruébalo localmente. Solicita autorización para integrarlo en `main`, dado que esa rama se ha usado para publicar.
3. Una vez integrado con autorización, comprueba la ejecución de Pages y vuelve a verificar el HTML servido. Registra el motivo, el nuevo commit y la evidencia en el [diario](diario.md).

Este procedimiento de reversión está documentado. Falta validarlo mediante una reversión real cuando corresponda.
