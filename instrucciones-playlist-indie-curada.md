# Cómo armar la "Playlist Curada Indie" con Claude

Este documento explica el flujo para que cualquier persona pueda replicar el proceso de curación semanal de música indie usando Claude + Spotify.

## Requisitos previos

1. Una cuenta de Claude.ai (Pro, Team o Enterprise; el conector de Spotify requiere un plan pago).
2. Conectar tu propia cuenta de Spotify en **Settings → Connectors**. Cada persona debe autorizar el acceso con su propia cuenta — este paso no se puede compartir ni transferir entre usuarios, es una medida de seguridad de OAuth.

## Instrucciones para pegar en Claude

Podés pegar esto directamente en un chat nuevo, o guardarlo como instrucciones personalizadas de un Project:

> Cuando me armes playlists de música indie, consultá primero NME, Stereogum, Indie Hoy, Pitchfork y Rolling Stone para ver qué están recomendando esa semana, y basá la selección en esas fuentes. La playlist debe tener 15 canciones y el nombre debe incluir la palabra "curada".

## Qué hace Claude con esto

1. Busca en la web las notas semanales de cada publicación (por ejemplo "The 5 Best Songs Of The Week" de Stereogum, "Songs You Need to Know This Week" de Rolling Stone, "Best New Tracks" de NME, listas de Indie Hoy, y reseñas recientes de Pitchfork).
2. Filtra las recomendaciones para quedarse con las que realmente encajan en indie rock/folk/pop (dejando afuera lo que es claramente de otro género, aunque la publicación lo haya cubierto esa semana).
3. Arma una lista de 15 canciones, tratando de repartir la selección entre las cinco fuentes.
4. Crea la playlist en Spotify (usando el conector) con un nombre que incluya la palabra "curada", por ejemplo: *"Curada Indie – Semana del [fecha]"*.

## Notas

- El resultado depende de qué publicaron esas fuentes esa semana en particular — si alguna no sacó una nota específica, Claude lo aclara en vez de inventar canciones.
- Si querés que el foco sea otro género o mezcle fuentes en español (Indie Hoy) con más peso, basta con decírselo a Claude en el chat.
- La playlist creada queda en la cuenta de Spotify de la persona que la pidió, no en la tuya.
