# Arquitectura técnica

[index.html](../index.html) reúne HTML, CSS, JavaScript nativo, datos y metadatos SEO. El repositorio carece de framework, compilación, dependencias instalables, código de servidor, CI y pruebas automatizadas.

## Flujos de la aplicación

- **Conversor.** Normaliza el importe de entrada y aplica la unidad en euros. Divide por el coste de referencia o, para gasto anual, por el importe diario calculado con 365 días. Muestra alcance y fuente. Genera una tarjeta PNG en Canvas y prepara texto para WhatsApp, X y Substack.
- **Histórico.** Combina catálogos del conversor con series adicionales. Busca y filtra observaciones y dibuja barras mediante el DOM. El ajuste habitual es `importe nominal × IPC de octubre de 2026 / IPC del año de referencia`. Algunas fichas ya traen el importe ajustado. Las notas por observación describen fuentes y aproximaciones.
- **Adivina.** Semilla determinista por fecha de `Europe/Madrid`. Guarda la partida y la cola de estadísticas opcionales en `localStorage`. El generador v3 se usa desde el 22 de noviembre de 2026. La versión del generador es independiente de la versión de la web.
- **Idioma.** Detecta el idioma del navegador. La interfaz inglesa conserva parte de los conceptos, notas y formatos en español.

## Servicios y publicación

- **Formspree.** Recibe el envío HTML de contacto con mensaje y, cuando se facilitan, nombre y correo. [prueba-contacto.html](../prueba-contacto.html) usa el mismo servicio.
- **Cloudflare Workers.** Recibe estadísticas del reto con consentimiento por partida. El cliente envía eventos con ID aleatorio, fecha y, para respuestas, tipo, acierto y tiempo aproximado. El código y la configuración del Worker quedan fuera de este repositorio.
- **Cloudflare Web Analytics.** Carga su propio script con independencia de la opción de estadísticas del reto.
- **Compartir y colaborar.** WhatsApp y X abren sus interfaces para compartir. Substack abre el perfil y usa el portapapeles. Ko-fi es un enlace de colaboración.
- **Dominio y rastreo.** [CNAME](../CNAME) declara el dominio. [robots.txt](../robots.txt) remite a [sitemap.xml](../sitemap.xml). Consulta [Estado](estado.md) para conocer qué se ha verificado del despliegue.
