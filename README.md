# Rotación de Puestos 2.0

PWA en español para organizar la rotación automática de cinco puestos y gestionar manualmente 5S y Team Lift.

## Novedades de la versión 2.0

- Water Spider: hasta 6 huecos (antes 5).
- Pusher: hasta 5 huecos (antes 4).
- 5S sale de la escala automática y conserva 6 huecos de asignación manual.
- Team Lift incorpora 6 huecos manuales: Feeder, Inductor, Water Spider, Stower 1, Stower 2 y 5S.
- Las asignaciones manuales se pueden editar de forma independiente en cada tramo. La plantilla sirve como punto de partida y se puede copiar a cada tramo.
- Cronómetros independientes para los cambios de Tramo 2 y Tramo 3, con límite de referencia de 10 minutos y contador de tiempo extra.
- Los cronómetros guardan el inicio y el tiempo acumulado en el dispositivo; si la aplicación se cierra mientras están en marcha, al volver a abrirla se calcula el tiempo transcurrido.
- Recomendación de orden de movimientos según una estimación relativa de recorrido y el sentido del cambio.
- La caché offline se actualiza a `rotacion-v2`.
- Se conserva la migración de la plantilla anterior guardada en el navegador.

## Publicación en GitHub Pages

Sube el contenido de esta carpeta a la raíz de la rama publicada (normalmente `main`) y configura Settings → Pages → Deploy from a branch → `main` → `/(root)`.

## Notas operativas

- La rotación automática conserva en los tres tramos la cantidad de personas por puesto definida en la plantilla.
- Se mantienen las validaciones existentes: Water Spider 1–6, Feeder e Inductor con la misma cantidad, Pusher 1–5 y Diverter 2–4.
- Los valores de distancia usados para priorizar movimientos son estimaciones relativas iniciales, no mediciones físicas. Conviene contrastar el orden sugerido con el recorrido real de la instalación y ajustar los pesos si se conoce la distribución exacta.
- La recomendación de orden no sustituye la coordinación del responsable ni garantiza por sí sola que cada puesto permanezca cubierto durante los movimientos.
- Es una PWA; GitHub Pages publica la aplicación web, no genera un APK nativo.
