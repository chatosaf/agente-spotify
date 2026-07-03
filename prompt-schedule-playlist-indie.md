# Prompt para /schedule en Claude Cowork

## Cómo usarlo
1. Abrí Claude Desktop → pestaña **Cowork**.
2. Escribí `/schedule` en el chat.
3. Cuando te pregunte qué querés automatizar, pegá el prompt de abajo.
4. Elegí la frecuencia (por ejemplo: semanal, jueves 10am).
5. Confirmá.

## Prompt

Todos los jueves a las 10am: consultá NME, Stereogum, Indie Hoy, Pitchfork y Rolling Stone para ver las recomendaciones de música indie de esa semana, y basá la selección en esas fuentes.

Antes de elegir las canciones, leé el archivo `~/Documents/playlist-historial.md` para ver qué canciones ya usé en semanas anteriores y evitar repetirlas. Si el archivo no existe, creálo.

Armá una selección de 15 canciones indie repartidas entre esas cinco fuentes. Creá una playlist en Spotify cuyo nombre incluya la palabra "curada", por ejemplo "Curada Indie – Semana del {date}".

Después, agregá esas 15 canciones (con la fuente de cada una) al final del archivo `~/Documents/playlist-historial.md`, para que la próxima corrida las pueda leer y evitar repetirlas.

## Notas
- Si alguna publicación no sacó una lista específica esa semana, que lo aclare en vez de inventar canciones.
- El requisito de 15 canciones y el nombre con "curada" están guardados en tus preferencias de Claude, así que se aplican también si le pedís la playlist manualmente en cualquier chat.
