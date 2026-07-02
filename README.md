# Agente de Playlist Curada para Spotify

**Trabajo Individual · MBA ORT Uruguay**  
**Materia:** Innovación y Estrategias de Tecnología  
**Alumno:** Luis Safons · N.º 90614

---

## ¿Qué es?

Un agente de IA que consulta semanalmente publicaciones especializadas de música, extrae sus recomendaciones editoriales y crea automáticamente una playlist curada de 15 canciones en Spotify.

El agente corre dentro de **Claude.ai** (Anthropic) y orquesta dos herramientas en tiempo real:

- **Web Search** — para leer qué están recomendando NME, Stereogum, Pitchfork, Rolling Stone e Indie Hoy esa semana
- **Spotify MCP** — para buscar esas canciones y crear la playlist directamente en la cuenta del usuario

---

## Flujo de trabajo

```
Usuario solicita la playlist
         ↓
Agente busca en NME, Stereogum, Pitchfork,
Rolling Stone e Indie Hoy (Web Search)
         ↓
Extrae artistas y canciones recomendadas
de la semana (razonamiento del LLM)
         ↓
Filtra por indie folk / indie rock / indie pop
         ↓
Busca cada canción en Spotify (MCP)
         ↓
Crea la playlist "Indie Curada · [Mes Año]"
en la cuenta del usuario
```

---

## Tecnologías

| Componente | Tecnología |
|---|---|
| Plataforma | Claude.ai (Anthropic) |
| Modelo de IA | Claude Sonnet |
| Búsqueda editorial | Anthropic Web Search Tool |
| Integración Spotify | Spotify MCP (Model Context Protocol) |

---

## ¿Qué es MCP?

Model Context Protocol (MCP) es un estándar abierto que permite a los agentes de IA conectarse a servicios externos (como Spotify) mediante "herramientas" que el modelo puede invocar durante su razonamiento. En este caso, el agente usa el conector MCP de Spotify para buscar canciones y crear playlists sin que el usuario maneje credenciales ni endpoints directamente.

---

## ¿Por qué es un agente y no un script?

Un **script de automatización** sigue una secuencia fija programada de antemano. Un **agente de IA** razona sobre qué pasos dar en función del objetivo:

- Decide qué buscar en cada publicación
- Interpreta resultados editoriales no estructurados
- Evalúa qué canciones encajan con el género pedido
- Ajusta la estrategia si los primeros resultados no son suficientes

El "código" de este agente no es un conjunto de instrucciones imperativas sino un **prompt** que define su objetivo, herramientas y criterios de decisión. Ver [`PROMPT.md`](PROMPT.md).

---

## Prompt del agente

El comportamiento del agente está definido por el prompt del sistema. Ver [`PROMPT.md`](PROMPT.md) para el texto completo.

---

## Resultado

Una playlist de 15 canciones creada directamente en la cuenta de Spotify del usuario, con canciones recomendadas esa semana por al menos una de las cinco publicaciones consultadas.

Ejemplo: **"Indie Curada · Julio 2026"** — curada a partir de Stereogum (Lily Seabird, Squirrel Flower, Slow Pulp), NME (Mitski, Aldous Harding, Lime Garden) e Indie Hoy (Anabel G.).

---

*Desarrollado con Claude.ai · Julio 2026*
