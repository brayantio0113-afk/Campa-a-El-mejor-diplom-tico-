# Plan de campaña comunicacional — Quiz ONU

## Objetivo

Aumentar el alcance y la participación en el quiz sobre el Consejo de Seguridad de la ONU, identificar qué red social trae a los usuarios más valiosos y usar el ranking para generar competitividad entre los participantes.

La campaña se basa en difusión de enlaces, medición con UTM, análisis de datos y optimización del canal que mejor funcione.

---

## Paso 1 — Infraestructura de medición y competitividad

La página está registrada en un servidor que recolecta información de los participantes:

- Jugadores que iniciaron el quiz.
- Jugadores que terminaron el quiz.
- Red social o canal desde el que llegó cada participante.
- Resultado obtenido.
- Interacción con el ranking.

La web cuenta con un sistema de ranking para crear competitividad entre los concursantes y motivar que más personas completen el quiz.

Además, se deben verificar los eventos mínimos de medición:

- `quiz_start`: el usuario inicia el quiz.
- `quiz_complete`: el usuario termina el quiz.
- `ranking_view`: el usuario consulta el ranking.

---

## Paso 2 — Creación de enlaces UTM por red y canal

Crear enlaces con UTM para extraer los datos de dónde viene la audiencia.

Cada red social o canal debe tener su propio enlace, sin reutilizarlo entre canales.

Ejemplos de canales:

- WhatsApp difusión.
- WhatsApp estados.
- WhatsApp contactos estratégicos o referidos.
- Facebook publicación.
- Facebook grupos.
- Instagram bio.
- Instagram stories.
- Discord.
- Reddit.
- Otras comunidades.

Convención recomendada:

- `utm_source`: red o canal.
- `utm_medium`: formato o tipo de publicación.
- `utm_campaign`: nombre de la campaña.
- `utm_content`: variante del mensaje, ronda o público.

Mantener una tabla de control con:

- Canal.
- Enlace UTM.
- Público al que se dirigió.
- Fecha automática registrada por el servidor.
- Clics o sesiones.
- Iniciados.
- Terminados.
- Tasa de finalización.
- Compartidos.

---

## Paso 3 — Implementar botón para compartir el resultado

Añadir en la web un botón de compartir resultado para que, al terminar el quiz, el usuario pueda publicar su puntuación, precisión o posición en el ranking.

El botón debe:

- Aparecer al finalizar el quiz.
- Mostrar un texto predefinido con el resultado.
- Incluir el enlace a la página.
- Permitir compartir en redes sociales o copiar el enlace.
- Registrar el evento `share_click` y, cuando sea posible, `share_complete`.

Texto sugerido:

> Obtuve [puntuación]% de precisión en este quiz sobre el Consejo de Seguridad de la ONU. ¿Puedes superarme en el ranking de diplomáticos?

Este paso convierte a los participantes en difusores del enlace.

---

## Paso 4 — Difusión del enlace en distintas redes

Compartir el enlace en distintas redes sociales y canales, usando siempre el UTM correspondiente a cada canal.

La difusión debe organizarse en dos rondas comparables, sin asignar días ni tiempos:

### Ronda A — Publicaciones dirigidas a cualquier público

Publicaciones abiertas en redes generales, estados de WhatsApp, publicaciones de Facebook e Instagram, entre otros canales de audiencia amplia.

Objetivo: medir el alcance general y la respuesta de un público no segmentado.

### Ronda B — Publicaciones dirigidas a público específico

Publicaciones en grupos, comunidades y contactos relacionados con:

- Modelos de Naciones Unidas.
- Relaciones Internacionales.
- Derecho.
- Ciencias Políticas.
- Geopolítica.
- Historia.
- Trivia y cultura general.
- Comunidades de Discord o Reddit afines.

Objetivo: comparar si el público específico responde mejor que el público general.

El servidor registra automáticamente la fecha de cada entrada

---

## Paso 5 — Análisis de datos y énfasis en la red que mejor funcione

Analizar los datos de las personas que entran y comparar el rendimiento por red y por ronda.

Métricas principales:

- Sesiones o clics por red.
- Jugadores que iniciaron el quiz.
- Jugadores que terminaron el quiz.
- Tasa de finalización: terminados / iniciados.
- Tiempo o profundidad de interacción
- Consultas al ranking.
- Clics en el botón de compartir.
- Compartidos completados.

Comparar especialmente:

- Ronda A: público general.
- Ronda B: público específico.

Según qué red funcione mejor, hacer énfasis en ella.

No priorizar solo los clics. Dar más peso a la red que traiga:

- Más jugadores que terminan el quiz.
- Mejor tasa de finalización.
- Más interacción con el ranking.
- Más compartidos del resultado.

---

## Paso 6 — Optimización del mensaje y del ranking

Ajustar el mensaje según los resultados del análisis.

Recomendaciones:

- Si el público general abre pero no termina, enfatizar el reto, la precisión y el ranking.
- Si el público específico termina más, reforzar la difusión en comunidades de MUN, Relaciones Internacionales y geopolítica.
- Resaltar visualmente el ranking, la precisión y la posibilidad de compartir el resultado.

---

## Paso 7 — Amplificación por referidos y comunidades

Pedir a las personas que ya completaron el quiz que compartan su resultado usando el botón de la web.

Acciones recomendadas:

- Compartir una captura del ranking personal.
- Pedir a contactos estratégicos que compartan el enlace con su propia red.
- Publicar en comunidades afines respetando sus reglas.
- Evitar spam y mensajes masivos repetitivos.
- Priorizar comunidades donde el tema sea relevante.

---

## Paso 8 — Seguimiento, privacidad y reporte

Mantener un panel simple de seguimiento con los datos recolectados por el servidor y los UTM.

Revisar:

- Qué red trae más iniciados.
- Qué red trae más terminados.
- Qué red tiene mejor tasa de finalización.
- Qué ronda funciona mejor: público general o público específico.
- Qué mensaje genera más compartidos.

Al finalizar la campaña, generar un reporte breve con:

- Redes utilizadas.
- Enlaces UTM.
- Iniciados y terminados por red.
- Tasa de finalización por red.
- Comparación entre público general y público específico.
- Red recomendada para futuras campañas.
- Ajustes recomendados para el quiz y el mensaje.