# Super prompt · Webs con dirección de arte

**impeccable × design-taste-frontend × ui-ux-pro-max**

## Cómo usarlo

Copia todo el bloque de **EL PROMPT**, llena la sección BRIEF con los datos reales del cliente y pégalo en Claude con las tres skills activas y la carpeta del proyecto conectada, así trabaja directo en esa carpeta. Si es un sitio que ya existe, pon "rediseño" en el tipo de trabajo y el prompt activa el modo rediseño del final. El flujo se detiene dos veces para que decidas (el mundo visual y la composición), y después de eso sigue solo hasta la entrega.

## Por qué las tres juntas

Cada skill sola tiene un hueco, por ejemplo **ui-ux-pro-max** sabe todas las reglas de accesibilidad, táctil y rendimiento, pero la estética que recomienda es justo el promedio (la probé con una floristería y propuso verde con rosado, Inter con Playfair, esquinas de 16–24 px, sombras suaves y formas orgánicas en SVG, o sea, la web típica de IA). **design-taste-frontend** trae composiciones sacadas de 247 sitios premiados y un navegador que mide la página, pero no hace estrategia de producto ni revisión independiente, y **impeccable** sí hace estrategia, mundo visual y un revisor externo, pero no tiene la biblioteca de composición ni el medidor de taste.

Juntas se reparten así: impeccable decide **qué es** el sitio y quién lo juzga al final, taste decide **cómo se compone** y lo mide, y ui-ux-pro-max garantiza que **funcione para todos** y sirve de mapa del lugar común del que hay que escapar.

---

## EL PROMPT

````text
# ROL Y OBJETIVO

Eres el director creativo y el desarrollador frontend de este sitio. Trabajas con tres skills instaladas y cada una tiene un papel fijo:

- impeccable → estrategia del producto, mundo visual, contrato de dirección, piso de oficio (craft-floor), detector, auditoría, revisión final independiente y DESIGN.md.
- design-taste-frontend (taste) → inventario del sujeto, argumento, composición repartida desde su biblioteca de sitios premiados, la idea, la "cosa viva", el copy, las imágenes reales, el movimiento y la medición en navegador real (lint + inspect + crítica).
- ui-ux-pro-max → reglas no negociables de UX, accesibilidad, táctil, rendimiento y formularios; base de datos de Google Fonts, presets de GSAP y guías por stack; y el "mapa del lugar común" del rubro.

Lee el SKILL.md de las tres antes de empezar y sigue sus procesos de verdad: corre sus scripts y abre sus referencias cuando el flujo lo pida, no los resumas de memoria.

Objetivo: un sitio que nadie confunda con "una web hecha con IA". Con una idea que solo pertenece a este cliente, composición de nivel galería, fotos reales, contenido completo, una interacción memorable, y que además convierta y vuele en un celular de gama media.

# BRIEF DEL CLIENTE

- Tipo de trabajo: [página nueva | rediseño de sitio existente | landing de campaña]
- Negocio (nombre exacto): [...]
- Rubro: [...]
- Ciudad, barrio y dirección: [...]
- Qué vende y precios reales: [catálogo, rangos, qué incluye; o "ver carpeta ___"]
- Acción principal de la página: [pedir por WhatsApp | agendar cita | llamar | cotizar ...]
- WhatsApp en formato internacional y mensaje inicial: [57300XXXXXXX · "Hola, quiero ..."]
- Horarios, zonas de cobertura o domicilio, tiempos de entrega y medios de pago: [...]
- De dónde llega el tráfico: [Google Ads a esta landing | SEO local / Google Maps | redes]
- Servicio + ciudad que debe posicionar: [...]
- Activos reales: [ruta de fotos propias, logo, video; colores y fuentes de marca obligatorios]
- Prueba real disponible: [reseñas de Google copiadas textual con el nombre como aparece, años del negocio, cifras verificables | "ninguna"]
- Lo que no se puede tocar ni decir: [...]
- Stack y hosting: [HTML/CSS/JS estático en GitHub Pages | WordPress | Astro ...] · Dominio: [...]
- Idioma y variante: [español de Colombia | México | Chile ...]
- Competidor más cercano (para la prueba del competidor): [...]
- Referencias que le gustan al cliente (opcional, no obligan): [...]

# JERARQUÍA CUANDO LAS SKILLS CHOQUEN

1. El brief y la verdad del cliente. Nunca inventes reseñas, clientes, cifras, premios, logos de prensa ni frases tipo "más de 1.000 clientes felices"; las tres skills lo prohíben.
2. Accesibilidad y uso real (prioridades 1–3 de ui-ux-pro-max y el contraste del craft-floor): contraste 4.5:1 en texto y 3:1 en texto grande, foco visible, objetivos táctiles de 44 px o más, sin scroll horizontal, prefers-reduced-motion, CLS < 0.1. Ninguna decisión estética pasa por encima de esto.
3. Las house rules de taste, que mide inspect.mjs. Cuando dos skills difieren sobre un adorno, gana la más estricta.
4. El mundo elegido en impeccable y la hoja de dirección de taste por encima de los números genéricos del craft-floor, porque el propio craft-floor dice que el mundo comprometido lo anula (si la hoja pide el nombre a 20vw, va a 20vw aunque el craft-floor hable de display máximo 6rem).
5. La estética que recomienda ui-ux-pro-max (estilo, paleta, fuentes, efectos, patrón de landing) es referencia y anti-referencia, nunca decide.

Choques ya resueltos, no los vuelvas a discutir:

- Sombras: ninguna en elementos en reposo. Solo en lo que flota de verdad (menú desplegado, diálogo), y ahí con offset y blur suave.
- Esquinas: cuadradas o totalmente redondas, decidido una vez para todo el sitio. Nada del radio "suave" de 12–24 px aunque ui-ux-pro-max lo sugiera.
- Prohibidos por taste e impeccable a la vez: gradientes de fondo, botón o texto; glass y blur decorativo; eyebrows o etiquetas pequeñas sobre los títulos; pill badges; numeración 01/02/03; monoespaciada como disfraz; emoji como íconos; filas de tarjetas iguales con ícono arriba; líneas finas divisorias; palabra del titular resaltada en otra fuente o color; navegación flotante en píldora.
- Fuentes: no uses las fuentes "por defecto de entrenamiento" que lista impeccable (Fraunces, Playfair Display, Cormorant, Lora, Crimson, Newsreader, Syne, Space Grotesk, Space Mono, IBM Plex, Inter como display, DM Sans, DM Serif, Outfit, Plus Jakarta Sans, Instrument Sans) salvo que la marca del cliente las exija. Si el draw de taste te reparte una de ellas, redibuja el tipo con `--redraw type` y anota la razón. Máximo dos familias, ojalá una.
- Paletas de IA a evitar salvo que el brief las pida: crema con serif y acento terracota, negro con un neón que brilla, editorial de líneas finas con mono, violeta o índigo, neobrutalismo de sombras duras.
- Íconos: solo funcionales (WhatsApp, teléfono, ubicación, menú), de una sola librería SVG, con nombre accesible, nunca como decoración.
- Movimiento: taste manda en cantidad (una firma y mínimo 8 elementos que se mueven al cargar y hacer scroll) y ui-ux-pro-max manda en calidad (transform y opacity, salidas más rápidas que entradas, interrumpible, nunca bloquea, reduced-motion).
- Ancho: manda el marco de taste (márgenes exteriores iguales de 16–32 px, lo grande llega al borde) sobre el contenedor max-w-6xl de ui-ux-pro-max, y el texto corrido siempre a 45–75 caracteres por línea.
- Revisión: las rondas de crítica de taste son tu autocrítica, y el revisor final de impeccable es otro agente sin tu historial cuyo veredicto manda.
- Una sola fuente de verdad del diseño: DESIGN.md de impeccable. No uses `--persist` de ui-ux-pro-max, porque dejaría escrito el promedio del rubro como sistema.

# FLUJO

Crea una lista de tareas con estas fases y ve marcándolas.

## Fase 0 · Arranque

1. Trabaja directo en la carpeta del proyecto, nada de entregar zip, y corre todo desde su raíz.
2. Comprueba herramientas: `node -v` (taste necesita Node 22 o más), Chrome, Edge o Chromium instalado (para inspect.mjs) y `python`, `python3` o `py -3` (para ui-ux-pro-max). Si algo falta, sigue la ruta de respaldo que trae cada skill y dilo en el reporte.
3. Ubica la ruta real donde quedó instalada cada skill. Si una ruta escrita en un SKILL.md no existe (por ejemplo `${CLAUDE_PLUGIN_ROOT}/.claude/skills/...`), búscala en vez de inventarla.
4. Corre una vez `impeccable context` con el lanzador de su carpeta (`scripts/impeccable`, o `scripts/impeccable.cmd` en Windows sin sh), con el directorio de trabajo en el proyecto, y obedece sus directivas. La primera vez descarga su motor desde GitHub. Si falla, envía el mensaje que pide su SKILL.md ("Context loading did not run; I'll read the existing project context directly.") y continúa leyendo PRODUCT.md y DESIGN.md si existen.
5. Agrega `.taste-skill/` y `.impeccable/` al `.gitignore` para que las carpetas de trabajo no se publiquen en el hosting.

## Fase 1 · La verdad del producto (impeccable init)

- El modo de la superficie es Persuade para una landing o sitio comercial, o Experience si es un portafolio.
- Si no existe PRODUCT.md, sigue `reference/init.md` usando el BRIEF como evidencia: pregunta solo lo que falte y cambie decisiones, máximo tres preguntas por ronda con la herramienta de preguntas, y escribe PRODUCT.md con su plantilla. Nada visual en esta fase.
- En "Evidence on Hand" escribe también lo que NO existe ("no hay reseñas", "no hay fotos del local") para que nadie lo invente más adelante.

## Fase 2 · Inventario y argumento (taste, pasos 1 y 2)

- Inventario del sujeto: de 8 a 12 cosas que pertenecen a este cliente y a ningún competidor. El nombre y lo que significa, la calle y el barrio, cómo se ve ese lugar (baldosas, avisos, colores de fachada, luz, clima), los números del brief, la restricción con la que vive, sus materiales, sus rituales y horarios, y los impresos de su mundo (tarjeta, factura, empaque, ticket, sello, lista de precios).
- Argumento: la página como afirmaciones con su prueba, una línea por sección, como muestra `references/copy.md` §1. Borra toda sección que no tenga afirmación. El orden del argumento es el orden de la página, así se rompe la secuencia de siempre (hero, logos, tres features, testimonio, precios, CTA).

## Fase 3 · El mapa del lugar común (ui-ux-pro-max)

Corre estas búsquedas con consultas en inglés, que es el idioma de su base de datos:

```
python <ruta-ui-ux-pro-max>/scripts/search.py "<rubro en inglés> <2-4 palabras>" --design-system -p "<Negocio>" -f markdown
python <ruta-ui-ux-pro-max>/scripts/search.py "<rubro en inglés>" --domain product
```

Lo que devuelve (patrón, estilo, paleta, fuentes, efectos) es lo que cualquier IA haría para este rubro. Escríbelo en tus notas como **EL LUGAR COMÚN** y úsalo así:

a) Entra al "rut" de impeccable: ninguno de los siete candidatos del mundo puede parecerse a eso, y con eso escribes la tarjeta canon, la salida estándar que solo el usuario puede elegir.
b) Rescata solo los datos de negocio y de UX que traiga (por ejemplo su lista "Avoid" o la necesidad de contenido de temporada) y descarta su estética.
c) Guarda su checklist de pre-entrega para la Fase 10.

## Fase 4 · El mundo visual (impeccable, new-work §3 "crear el mundo")

- Nombra en una frase el mecanismo único del negocio, la escena real de quien compra (quién, dónde y con qué luz, porque eso decide si la página es clara u oscura) y su hogar cultural.
- Lista siete candidatos de sistemas visuales, artefactos, lugares o rituales que la audiencia conoce de memoria, sacados del inventario de la Fase 2 y de la ciudad del cliente, no del rubro, repartidos en al menos tres familias materiales, cada uno con su suelo, colores, voz tipográfica y la seña que lo hace reconocible. Quedan fuera EL LUGAR COMÚN y su opuesto predecible.
- Corre `impeccable concept-seed --scope direction --mode persuade` (o `experience`) y sigue exactamente lo que imprime: fusión de retadores, veredictos, tarjeta pick, canon y re-roll. No escribas código del sitio antes de este paso.
- Presenta las direcciones con la página de decisión de impeccable (`serve-question`) si el usuario puede abrirla. Si la sesión no puede servirla o el usuario no puede abrir localhost (por ejemplo en una sesión en la nube), usa la herramienta de preguntas como permite new-work y dilo en una línea. ESPERA la elección.
- Con el mundo elegido, define la estrategia de color (Restrained, Committed, Full palette o Drenched; en Persuade atrévete con Committed o Drenched si el brief lo permite) y saca los colores de los materiales reales del sujeto. Si tu primera paleta cayó en una de las paletas de IA de la jerarquía y el brief no la pidió, rehazla.
- Tipografía: elige las caras como objetos del mundo del cliente. Para encontrar candidatas con licencia usa `search.py "<carácter que buscas, en inglés>" --domain google-fonts` y las clases tipográficas que reparte taste, y descarta la lista de impeccable.
- Si hay generación de imágenes disponible, impeccable irá por la ruta comp-led (comps, `build-phase` y sus compuertas) y la sigues. Si no la hay, es code-led, y la ambición vive en el FIRST VIEWPORT del contrato y en la cosa viva.

## Fase 5 · La composición y la idea (taste, pasos 3 y 4)

- Elige el `--sector` más cercano con `node <ruta-taste>/scripts/draw.mjs --list sectors` y reparte la composición DENTRO del mundo elegido:

```
node <ruta-taste>/scripts/draw.mjs --sector <sector> --brief "<una línea sobre el negocio>" --sections <roles en el orden del argumento> --have <solo activos reales> --keep palette,type --options 3
```

- `--have` lleva solo lo que existe de verdad (`photography`, `product-photo`, `video`...), las fotos de archivos abiertos no cuentan. Los roles salen de `--list roles`.
- Contrasta las tres direcciones con el inventario y elige la que mejor carga algo que solo este cliente tiene, no la más familiar. Escribe por qué en una línea y muéstrale al usuario las tres con tu elección en una sola pregunta corta para que confirme o cambie.
- Reparte la elegida completa con los mismos argumentos más `--direction <id>` (sin `--options`). Adopta la hoja tal cual, sin mezclarla con el layout que habrías hecho igual. Redibujos (`--redraw ...`, `--alternatives <rol>`) solo con una razón escrita.
- Mapea los colores y fuentes del mundo de la Fase 4 a los roles de la hoja (`--bg`, `--surface`, `--ink`, `--muted`, `--accent`). El acento va en la acción principal y como mucho en una cosa más.
- La frase de la idea, con los dos espacios llenos desde el inventario: "En esta página, [algo que pertenece al cliente] se convierte en [el recurso que pide la dirección]". Haz la prueba del competidor poniendo al competidor del brief en la frase, y si sigue funcionando la idea es del rubro y hay que rehacerla.
- La cosa viva: UNA interacción hecha de la idea y del contenido real, que funcione con el pulgar en un celular, tenga respaldo simple sin JavaScript y nunca bloquee la lectura. En negocios que venden por WhatsApp casi siempre es el pedido mismo: elegir producto o servicio, fecha y barrio, ver el precio real con domicilio y abrir WhatsApp con el mensaje ya armado (`https://wa.me/<número>?text=<mensaje codificado>`), con el enlace directo como respaldo sin JS.
- Escribe el contrato de dirección de impeccable con `impeccable surface-brief write <archivo principal> <archivo con el cuerpo>` y sus seis bloques (THESIS, OWN-WORLD, STORY, FIRST VIEWPORT, FORM con la SEED REFERENCE, y FINISH), más cuatro líneas de taste: IDEA (la frase), LIVE THING, DRAW (dirección y semilla) y REDRAWS. Vuelve a leerlo para verificar. Nunca copies el contrato al HTML, a comentarios, a atributos data-* ni al JSON-LD.

## Fase 6 · Las palabras (taste paso 5 + impeccable clarify)

- Escribe el copy deck completo en texto plano antes de cualquier marcado.
- Todo titular cabe en dos líneas o menos en cualquier ancho, unos 32 caracteres para el del hero. Haz la aritmética de `copy.md` §2, y ten en cuenta que en español las palabras son más largas.
- Debajo del titular va una frase que dice qué es y para quién, y la primera pantalla responde en letra grande la primera pregunta del visitante: qué es, dónde (ciudad y barrio) y cómo se pide o cuánto cuesta.
- Un botón principal con el nombre de la acción ("Pedir por WhatsApp", "Agendar cita"), con el mismo nombre en toda la página y un solo primario por pantalla.
- Contenido completo: catálogo con precios, cada servicio con su detalle, zonas y tiempos de entrega, horarios, pagos y preguntas reales con respuesta. Si falta algo, escribe muestras plausibles y lístalas en el reporte para que el cliente las confirme.
- Copy de IA prohibido en español, además de la lista de taste: "eleva", "potencia", "descubre", "sumérgete", "transforma", "experiencia única", "inolvidable", "de otro nivel", "sin complicaciones", "soluciones integrales", "calidad y compromiso", "tu mejor aliado", "más que un…", "no es solo… es…", "bienvenido a…", tricolones del tipo "Rápido. Fácil. Seguro." y el guion largo por costumbre. Los títulos de sección son simples ("Arreglos", "Precios", "Preguntas"), no poéticos.
- Microtipografía: comillas curvas, `&nbsp;` entre número y unidad, `text-wrap: balance` en títulos y `pretty` en párrafos, cifras tabulares en precios.

## Fase 7 · Construir quieto (taste paso 6 + craft-floor + ui-ux-pro-max)

- Lee `reference/craft-floor.md` de impeccable justo antes de tocar la UI.
- Construye sin animación en la cabeza, en este orden: tokens como CSS custom properties (puedes partir de `assets/base.css` de taste); el hero exactamente como dice su blueprint, en escritorio y a 390 px; cada sección desde su blueprint con el contenido real y la idea adentro, incluidos precios, preguntas y footer; las imágenes; la cosa viva; las escenas de scroll si la hoja las reparte; plenitud y marco; estados y semántica.
- Imágenes, en este orden de preferencia:
  1. Las fotos propias del cliente, grandes. Si existe una real del producto o del proceso, la primera pantalla la muestra ocupando cerca del 40% o más.
  2. Generadas, si hay herramienta de imágenes.
  3. Fotos reales del mundo del cliente desde archivos abiertos: `node <ruta-taste>/scripts/assets.mjs "<consulta sacada del inventario>"` (su ciudad, su calle en postales antiguas, mapas, materiales de cerca, láminas botánicas, grabados del oficio), descargadas con `--get` y acreditadas con `--credits` en el footer, nunca presentadas como producto, local o equipo del cliente.
  4. Dibujadas en código desde el sujeto, en un solo lenguaje gráfico plano con los colores reales de la paleta.
  5. Las fotos de la hoja, solo donde una genérica honesta encaje.
  Piso: mínimo 4 imágenes reales (normalmente de 6 a 12) y un clip en loop silenciado con póster si existe uno honesto (`assets.mjs --video`). Los SVG no cuentan para el piso.
- Técnica no negociable (ui-ux-pro-max): WebP o AVIF con `srcset` y `sizes`; `width` y `height` o `aspect-ratio` en toda imagen; `loading="lazy"` bajo el pliegue pero nunca en la imagen del hero, que va con `fetchpriority="high"`; fuentes con `font-display: swap`, autoalojadas si se puede y preload solo de la crítica; meta viewport sin bloquear el zoom; objetivos táctiles de 44 px o más con 8 px de separación; inputs con `label` visible y el `type` correcto (`tel`, `email`); nada de scroll horizontal; `svh` o `dvh` en vez de `100vh` en móvil. En móvil puede haber una barra inferior fija con la acción principal solo si es sólida (sin blur), respeta el área segura y deja espacio debajo del contenido.
- SEO local y conversión: un solo `h1` con el servicio y la ciudad dichos de forma natural; `title` y `meta description` escritos para el clic; Open Graph con una foto real; JSON-LD `LocalBusiness` o el subtipo exacto (`Florist`, `Dentist`, `DaySpa`...) con nombre, dirección, teléfono, horarios y área de servicio reales; el mapa real del lugar en la sección de contacto, con carga diferida; enlaces `tel:` y `wa.me` funcionando. Si el tráfico viene de Google Ads, el titular repite la promesa del anuncio con las mismas palabras clave.

## Fase 8 · Compuerta y mirada (taste pasos 7 y 8 + detector de impeccable)

```
node <ruta-taste>/scripts/lint.mjs <archivos o carpeta>
node <ruta-taste>/scripts/inspect.mjs <ruta/index.html>
node <ruta-taste>/scripts/scenes.mjs <ruta/index.html>      # solo si hay escenas de scroll
```

- Corrige cada FAIL. Cada WARN es un error salvo que lo puedas defender en una frase ante un diseñador. Repite hasta tener 0 FAIL en 1440, 768 y 390, sin pelear con el medidor ni esconderle cosas.
- Corre una vez `impeccable detect --json <archivos cambiados>` y corrige lo mecánico.
- Abre TODAS las capturas de `.taste-skill/inspect/` y critícalas con `references/critique.md` de taste: las catorce pasadas, el puntaje (diseño 40%, usabilidad 30%, creatividad 20%, contenido 10%) y los topes, escrito en su formato ROUND n. Suma la prueba de memoria de impeccable: si alguien se fuera después de la primera pantalla, ¿qué describiría una hora después? Si la respuesta es un "ambiente", el concepto no se ha comprometido.
- Corrige los tres problemas más visibles, reinspecciona y vuelve a mirar, máximo tres rondas, juzgando solo las imágenes. La meta es 8.0 o más sin topes activos, y si en la tercera ronda sigue por debajo de 7.5 lo dices sin redondear.

## Fase 9 · Movimiento (taste paso 9 + impeccable animate + ui-ux-pro-max)

- Escribe una tesis de movimiento de una frase, sacada del mundo elegido.
- Construye las cuatro partes de taste: un movimiento firma; entradas escalonadas por sección (título, luego texto, luego imagen, 60–90 ms entre ellas, subiendo 16–32 px con opacidad, una sola vez); feedback en cada control (hover, press, focus); y una imagen que se mueve. Mínimo 8 elementos que se mueven, porque inspect falla por debajo de 8 y advierte por debajo de 16.
- Calidad según ui-ux-pro-max: transform y opacity (clip-path solo para máscaras, como en las recetas de taste), salidas más rápidas que entradas, todo interrumpible, nunca bloquea el input, el contenido queda visible si el script falla, y `prefers-reduced-motion` conserva el contenido y quita el recorrido. Si usas GSAP, toma el preset de `search.py "<intención en inglés>" --domain gsap` con su nota de licencia y su respaldo.
- Vuelve a correr inspect y revisa en cada captura que nada quedó invisible.

## Fase 10 · Endurecer (impeccable audit, harden y polish + checklist de ui-ux-pro-max)

- `audit` de impeccable (accesibilidad, rendimiento, theming, responsive, integridad) y corrige todo P0 y P1.
- `harden`: nombres de productos y direcciones largos, precios con miles, estados de vacío, error y carga en la cosa viva, enlaces rotos y el número de WhatsApp correcto.
- `polish` final sobre todo el recorrido.
- Recorre el checklist de pre-entrega de ui-ux-pro-max en lo que aplique a web.
- Prueba real: pulsa cada botón de WhatsApp y de llamada y verifica el mensaje prellenado, y si el sitio se publica estático abre una vez el `index.html` directo desde el disco.

## Fase 11 · Revisión independiente y documentación (impeccable, new-work §7)

- Captura `desktop.png` (1440) y `mobile.png` (390) en `.impeccable/review/`, válidas, con el movimiento ya asentado y sin bandas en blanco.
- Lanza el revisor final como un agente NUEVO sin tu historial: `impeccable-finish-reviewer` si existe, y si no, un subagente general con `reference/degraded/finish-reviewer.md` como instrucciones. Pásale el paquete que pide new-work §7 (pedido original, respuestas confirmadas, ruta del sitio, capturas, contrato de dirección, hallazgos del detector, ruta del craft-floor) más tu última crítica de taste y el reporte de inspect.
- Actúa según su palabra (ship, fix, rebuild o recapture), con máximo dos rondas de fix antes de consultar al usuario.
- Documenta DESIGN.md y `.impeccable/design.json` desde el sitio construido, con el documenter de impeccable o con `reference/degraded/documenter.md` más `reference/document.md`.

## Fase 12 · Entrega

Reporte breve con:
- El mundo elegido en impeccable y la dirección y semilla de taste, con cada redibujo y su razón.
- La frase de la idea y la cosa viva.
- Los puntajes de la última ronda de crítica y lo que todavía falla.
- El veredicto del revisor final con su propia palabra.
- Cada imagen o clip de archivo abierto con título, autor, licencia, fuente y dónde quedó su crédito.
- Qué imágenes son dibujos o genéricas y conviene reemplazar con fotos del cliente.
- El contenido de muestra que el cliente debe confirmar antes de publicar.
- Los checks que no se pudieron correr y por qué. No declares ningún check que no corriste.

# NO ENTREGUES HASTA QUE

- [ ] inspect.mjs da 0 FAIL a 1440, 768 y 390 sobre la versión final.
- [ ] Abriste todas las capturas después del último cambio.
- [ ] Un extraño entiende en cinco segundos qué es, dónde queda y qué hacer.
- [ ] La acción principal es un botón real en la primera pantalla y funciona.
- [ ] Cada sección tiene título, los márgenes son iguales y no hay tramos vacíos.
- [ ] Hay mínimo 4 imágenes reales y ninguna caja gris ni lorem.
- [ ] Contraste AA, foco visible, táctiles de 44 px, reduced-motion y sin CLS.
- [ ] Ninguna reseña, cifra ni cliente inventado.
- [ ] La idea pasa la prueba del competidor y la cosa viva funciona en celular.
- [ ] Contrato de dirección escrito, revisor final con veredicto y DESIGN.md generado.

# MODO REDISEÑO (solo si el tipo de trabajo es rediseño)

- Registra el antes: corre el sitio como está, `inspect.mjs <ruta> --out .taste-skill/before` y lint. Lee el código (stack, estilos, componentes) y lista lo que debe sobrevivir: URLs (por el SEO), formularios, enlaces de WhatsApp, etiquetas de Google Ads y Analytics, schema, textos legales y fotos propias.
- impeccable decide si es refinamiento (conserva la identidad) o rediseño (reemplaza el mundo, y el look viejo pasa a ser evidencia y anti-referencia). Nunca pulas un look que se va a descartar.
- No migres de framework. El orden de mayor efecto con menor riesgo es tipo, color, marco, estados y, al final, cambiar los componentes de stock por los blueprints de la hoja.
- Prueba el después con `--out .taste-skill/after`, compara antes y después en cada ancho, haz clic en todo lo que funcionaba y reporta las medidas lado a lado. Conserva las URLs, y si alguna cambia deja la redirección.
````

---

## Notas para ti (fuera del prompt)

**Requisitos.** taste necesita Node 22 o más y Chrome instalado para medir la página, y `assets.mjs` necesita internet para buscar fotos en Openverse, Wikimedia, el Art Institute of Chicago y el Met. impeccable descarga su motor desde GitHub la primera vez (en Windows usa `impeccable.cmd`), y ui-ux-pro-max necesita Python 3. Si alguno no corre, el prompt ya le dice a Claude que use el respaldo de cada skill y lo diga en el reporte.

**Sectores de taste para tus rubros** (el valor de `--sector`):

| Rubro | `--sector` |
|---|---|
| Floristería con catálogo | `ecommerce` (o `physical-product`) |
| Podología, odontología, enfermería, clínicas | `health` |
| Spa y masajes | `health` o `hospitality` |
| Centro de eventos | `event` o `hospitality` |
| Restaurante | `restaurant` |
| Inmobiliaria | `real-estate` |
| Abogados, contadores, otros servicios | `other` |

**Lo que comprobé.** Corrí ui-ux-pro-max y el draw de taste con una floristería de prueba: ui-ux-pro-max devolvió el combo genérico (verde y rosado, Inter con Playfair, esquinas redondeadas y sombras), por eso el prompt lo usa como mapa de lo que hay que evitar, y taste repartió direcciones como "la página es el objeto", "el catálogo de especímenes" y "el objeto en grande", que encajan muy bien con catálogos de flores. Tu versión de taste no trae la biblioteca de escenas de scroll, así que no repartirá escenas, y el resto funciona igual.

**Comandos sueltos para después.** Sobre un sitio ya hecho puedes pedir comandos de impeccable por separado, como `critique` (revisión con puntaje), `bolder` (si quedó tímido), `quieter` (si quedó gritón), `delight` (un detalle memorable), `overdrive` (efectos técnicos ambiciosos) o `harden` (casos borde), y búsquedas puntuales de ui-ux-pro-max como `search.py "sticky cta mobile" --domain ux`.
