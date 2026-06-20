# Aniversario 2 🍄💞

Juego tipo Super Mario, hecho como regalo de aniversario. 6 mundos, cada uno
esconde una pregunta de nuestra historia dentro de un bloque **? ROSA**.

## Cómo se juega
- Mover: **← →** (o los botones en pantalla en celular). Saltar: **↑ / Espacio**.
- Hay que **sacar TODOS los bloques `?`** de cada mundo (golpéalos con la cabeza saltando desde abajo).
- El bloque **? ROSA** lanza la pregunta: hay que responderla bien.
- Sin sacar todos los `?` y responder, **la bandera 🏁 queda cerrada**.
- **1 vida ❤️ por día**: si se pierde, se repone al día siguiente (se guarda en el navegador).
- Arranca en el **Mundo 6** (los mundos 1–5 ya quedan pasados).

## Las preguntas
1. México 🌵 — ¿Dónde nos conocimos? → *rancho mx*
2. El Bosque — ¿Color favorito de Charlie? → *café*
3. Las Oficinas 🏢 — ¿Empresa de Charlie? → *didimosoft*
4. La Cocina 🍽️ — ¿Comida favorita de Charlie? → *garbanzos*
5. El Futuro 👶 — ¿Cómo se va a llamar nuestra hija? → *juanita*
6. El Equipo 👷 — Nombra DOS trabajadores de Charlie (necesita dos) → *carlos / jhampier / omar / fredy / paula(ita) / ivan*
7. El Gran Final 🎁 — ¿Qué crees que es tu primer regalo? (opción múltiple) → *Ropa*

## Estructura
Es un sitio **100% estático**: un solo `index.html` (sin build, sin dependencias).

## Subir a Vercel
Opción A — desde la web:
1. Sube esta carpeta a un repo de GitHub.
2. En vercel.com → *Add New → Project* → importa el repo.
3. Framework Preset: **Other**. Build Command: *(vacío)*. Output Directory: *(vacío / raíz)*.
4. Deploy. Queda un link público para compartir por WhatsApp.

Opción B — con la CLI:
```
npm i -g vercel
cd mario-hongos
vercel        # primer deploy (preview)
vercel --prod # a producción
```

> El guardado de vidas/progreso usa `localStorage` del navegador del jugador,
> así que funciona perfecto en el dominio de Vercel (cada persona guarda lo suyo).
