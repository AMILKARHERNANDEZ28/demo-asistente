# Demo de asistente IA (WhatsApp simulado)

Una sola página (`index.html`) y un archivo de configuración por cliente en `c/`.

- Enlace de cada cliente: `<dirección de la página>/?c=<id>`
- Sin `?c=` o con un id que no existe, la página solo muestra un mensaje neutro (no revela la lista de clientes).

## Agregar un cliente nuevo
1. Copiar `c/lb7k2.json` con un id nuevo, poco adivinable (letras minúsculas y números, por ejemplo `rz4p9.json`).
2. Cambiar nombre, saludo, sede, horario, horas ofrecidas, intenciones (palabras clave → respuesta) y el bloque de urgencia.
3. Poner el logo en `c/<id>-logo.jpg` (160×160) y apuntar `"logo"` a ese archivo.
4. Subir los cambios. El enlace queda `.../?c=<id>`. Generar el QR con ese enlace.

## Notas
- Las respuestas son guionadas (palabras clave), no IA real: sirve para demostrar el flujo sin riesgos.
- Los botones que muestra (horarios, Confirmar/Reprogramar, Dejar reseña) existen en la API oficial de WhatsApp.
- La página tiene `noindex` para que no aparezca en buscadores.
