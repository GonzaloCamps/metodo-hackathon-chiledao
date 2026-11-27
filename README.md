# Método Hackathon ChileDAO

**De la idea a la especificación, y de ahí a la entrega: gratis o con NoahAI.**

Este repositorio es para quienes participan desde Chile en la Dev3pack Global Hackathon sobre Solana, del viernes 27 al domingo 29 de noviembre de 2026. Es un método en cinco pasos para llegar de una idea propia a un proyecto entregado, aunque nunca hayas construido sobre una blockchain. Los cuatro primeros pasos van antes de lo técnico: encontrar la idea, validarla, evaluarla con los criterios del jurado y convertirla en una especificación. El quinto explica dos rutas para construir y entregar: una gratis y otra con NoahAI.

## Quiénes estamos detrás

**ChileDAO** es una comunidad abierta para aprender e impulsar el uso de IA y blockchain en Chile. Nació en 2025 y hoy organiza hackathones, talleres y eventos, y acompaña a empresas y proyectos que quieren entrar a Chile y Latinoamérica. Desde junio de 2025 ha organizado 22 eventos, más de 1.000 personas siguen sus actividades en Luma y 200 participan en su grupo de WhatsApp. Nos juntamos todos los martes a las 19:00, por Discord, y estamos conformando una cooperativa de trabajo para aportar a la transformación digital de Chile.

- **[Síguenos en redes desde nuestro Linktree](https://linktr.ee/web3chile):** ahí están Instagram, X, LinkedIn, Telegram y el Discord de las reuniones de los martes.
- **[Entra al grupo de WhatsApp de ChileDAO](https://chat.whatsapp.com/IU38ZwHD8MIFMrB11WbNxt):** ahí avisamos de cada actividad y se resuelven dudas.

**Dev3pack** es la comunidad global que organiza la hackathon. Forma a nuevas personas que construyen en Web3 e IA, con foco en quienes están menos representadas en el mundo de la tecnología, y tiene fuerte presencia en el sur global, con sedes en África, Asia y América Latina. Esta edición de la hackathon tiene sedes en 24 países. Sus sesiones y bootcamps están en su [canal de YouTube](https://www.youtube.com/@dev3pack).

Este método lo armó ChileDAO, que organiza la Build Station de Santiago, con las reglas de la hackathon, lo que enseñaron las sesiones de preparación y sus propias pruebas.

## Si partes de cero: qué es una blockchain y por qué Solana

Una blockchain es un registro compartido que no depende de una sola empresa ni de un solo servidor. Muchos computadores guardan la misma copia y validan cada cambio, así que lo que queda escrito no se puede borrar ni alterar a escondidas. Sobre ese registro se escriben programas, también llamados contratos inteligentes, que cumplen sus reglas solos: mueven dinero, registran quién es dueño de algo o dejan una constancia pública.

Aprender a construir sobre una blockchain te sirve más allá de este fin de semana. Es la base de los pagos digitales, de los activos tokenizados y de los agentes de IA que pagan por su cuenta, y todavía pocas personas saben hacerlo.

Solana es una blockchain que rinde bien en lo que más pesa para una app:

- **Es rápida:** produce un bloque cada 0,4 segundos, aproximadamente.
- **Es barata:** cada transacción cuesta una fracción de centavo de dólar.
- **Tiene con qué construir:** herramientas, documentación y una comunidad activa, también en español.

Por eso sirve para apps que la gente usa todos los días, y no solo para mover montos grandes.

Por ahora basta con eso. En el paso 2 del método vas a volver a la pregunta «¿por qué en Solana?», esta vez con tu propia idea: qué hace la blockchain en tu app que una app normal no puede, y cómo aprovecharla mejor.

Si quieres la base completa en español, está la clase [Basics of Blockchain](https://www.youtube.com/watch?v=gZLBW0FJbHk) del Solana Rust Bootcamp de Dev3pack.

## Qué vas a encontrar

El método son cinco pasos, uno por archivo. Cada paso termina con un resultado concreto, que es el punto de partida del siguiente.

| Paso | Archivo | Qué haces | Con qué terminas |
| --- | --- | --- | --- |
| 1 | [01-la-idea.md](01-la-idea.md) | Buscas una idea que salga de tu contexto: tu red, tu experiencia y los problemas que ves | El problema y el usuario, en dos frases |
| 2 | [02-validar.md](02-validar.md) | Revisas si ya existe, por qué ahora y por qué en Solana | Lo que existe, tu diferencia y por qué Solana, en tres líneas |
| 3 | [03-pauta.md](03-pauta.md) | Evalúas tu idea con las señales que mira el jurado | Tus puntajes y la propuesta de valor en una frase |
| 4 | [04-especificacion.md](04-especificacion.md) | Acotas la idea a dos días y la conviertes en una especificación | La especificación, lista para construir |
| 5 | [05-construir-y-entregar.md](05-construir-y-entregar.md) | Construyes por la ruta gratis o con NoahAI, y entregas | El programa en devnet, el repositorio público, la app publicada y el video |

Además:

- **[00-instrucciones-para-tu-ia.md](00-instrucciones-para-tu-ia.md):** los pasos 1 a 4 en un solo texto para pegar en una IA, que te guía con preguntas. Es la forma recomendada de usar el método.
- **[ejemplos/ruta-del-hacker.md](ejemplos/ruta-del-hacker.md):** un ejemplo completo, de la ficha a la especificación: una app para sellar tu idea y registrar tu ruta hasta la entrega.
- **[referencias/](referencias/):** los ganadores de la edición anterior y las ideas que el ecosistema de Solana quiere ver construidas.

## Por qué existe

En la [sesión del martes 24](https://www.youtube.com/watch?v=cMhjoZOhM0Q), Santiago mostró que NoahAI rinde más como ejecutor: la idea se piensa en otra IA, y a NoahAI se le entrega una especificación ya cerrada. En su demo gastó cerca de 2 millones de créditos y el programa no alcanzó a quedar listo. Tus créditos son limitados: piensa primero y construye después.

El jueves 26, Dev3pack avisó por correo que los créditos de NoahAI para la hackathon se agotaron: ya los habían canjeado 1.000 personas, y desde entonces solo hay un 30 % de descuento en NoahAI. Por eso el Método tiene ahora una ruta gratis: una IA gratuita escribe el programa y se despliega en devnet con Solana Playground, desde el navegador. Pensar primero sirve igual en las dos rutas. Ese mismo jueves, en su [sesión de consejos](https://www.youtube.com/watch?v=S9LyP7V82UQ), la organizadora de la hackathon recomendó lo mismo: antes de construir, pídele a una IA un prompt claro de lo que quieres hacer.

## Cómo usarlo

### Con tu IA (recomendado)

1. Abre ChatGPT, Claude, Gemini u otra IA. Sirve la versión gratuita.
2. Abre [00-instrucciones-para-tu-ia.md](00-instrucciones-para-tu-ia.md), copia todo lo que está bajo la línea y pégalo en tu IA.
3. Responde sus preguntas. Te guía por la idea, la validación, la pauta y el alcance, y al final te entrega la especificación.
4. Revisa la especificación línea por línea antes de construir.
5. Sigue con [05-construir-y-entregar.md](05-construir-y-entregar.md): ahí están las dos rutas para construir, la gratis y la de NoahAI.

Si tu IA puede abrir enlaces, también puedes darle el link de este repositorio.

### Leyéndolo

Sigue los archivos en orden, del 01 al 05. La tabla de «Qué vas a encontrar» dice qué haces en cada uno y con qué terminas.

### Referencias

| Archivo | Para qué |
| --- | --- |
| [referencias/ganadores-mayo-2026.md](referencias/ganadores-mayo-2026.md) | Los 30 finalistas y los ganadores por track de la edición de mayo de 2026, ordenados por tipo de proyecto, con los proyectos chilenos |
| [referencias/requests-for-startups.md](referencias/requests-for-startups.md) | Las once Requests for Startups de Solana: qué productos quiere ver construidos el ecosistema y por dónde empezar |

## Videos de Dev3pack

Las sesiones de preparación y el Solana Rust Bootcamp están en el [canal de YouTube de Dev3pack](https://www.youtube.com/@dev3pack). Estos son los que más sirven para seguir el método:

| Video | Idioma | Para qué paso |
| --- | --- | --- |
| [Basics of Blockchain](https://www.youtube.com/watch?v=gZLBW0FJbHk) | Español | Antes de partir: la base de qué es una blockchain |
| [Product Ideation: how to find real ideas](https://www.youtube.com/watch?v=yM6HUVMjxdI) | Inglés | Pasos 1 y 2: encontrar y validar una idea propia |
| [Vibecode your first app on Solana](https://www.youtube.com/watch?v=cMhjoZOhM0Q) | Inglés | Pasos 4 y 5: planificar con una IA y construir con NoahAI |
| [Enable micro-payments with x402 on Solana](https://www.youtube.com/watch?v=BoqpFVoYWQg) | Inglés | Paso 1, si tu idea usa pagos de agentes |
| [Deployment + Tips & Tricks](https://www.youtube.com/watch?v=ZWlm8H3htKc) | Español | Paso 5: el despliegue de un programa |
| [Best tips for your first hackathon](https://www.youtube.com/watch?v=S9LyP7V82UQ) | Inglés | Paso 5: qué pesa al evaluar y cómo entregar |

El Solana Rust Bootcamp completo en español, con sus 9 clases, está en [esta lista de reproducción](https://www.youtube.com/playlist?list=PLYPe1V-xMITw).

## Reglas que conviene tener presentes

- Se puede usar IA y plantillas, siempre que el proyecto sea tuyo.
- Hacer fork del proyecto de otro equipo y presentarlo como propio descalifica. Este repositorio es una guía: no lo entregues como proyecto.
- Puedes partir con código propio de un proyecto anterior en Solana, si le agregas funciones durante la hackathon y en el README cuentas qué existía y qué hiciste.
- La entrega cierra el domingo 29 a las 04:00, hora de Chile.

Si algo cambia en la hackathon, manda lo que diga el panel de Dev3pack.

## Dónde pedir ayuda

- [SoleneGPT](https://solenegpt.bonfires.ai/), el mentor de IA de la hackathon, en tu idioma.
- La pestaña Mentors del panel: filtra por país, idioma y habilidades.
- El [grupo de Telegram de la hackathon](https://t.me/+rlBixDYGfig1Zjc8).
- La Build Station de Santiago, el viernes 27 de 13:00 a 18:00 en la UDP: [inscripción en Luma](https://luma.com/ovbwi0fj).
- El panel de Dev3pack y sus [preguntas frecuentes](https://hack.dev3pack.xyz/faq): la organizadora avisó que desde el viernes no alcanza a responderle a cada persona, y que casi todas las respuestas están ahí.

## Fuentes

- Reglas, evaluación y proyectos de mayo de 2026: sitio, FAQ y panel de Dev3pack, revisados por ChileDAO el 23 de noviembre de 2026.
- [Hilo de Dev3pack con los ganadores de mayo de 2026](https://x.com/dev3pack/status/2053882621453811945) y [Requests for Startups de Solana](https://solana.com/es/request-for-startups), revisados el 24 de noviembre de 2026.
- Sesión [«Product Ideation: how to find real ideas»](https://www.youtube.com/watch?v=yM6HUVMjxdI), lunes 23 de noviembre, con Deepesh y Solene.
- Sesión [«Vibecode your first app on Solana»](https://www.youtube.com/watch?v=cMhjoZOhM0Q), martes 24 de noviembre, con Santiago.
- Sesión [«Enable micro-payments with x402 on Solana»](https://www.youtube.com/watch?v=BoqpFVoYWQg), miércoles 25 de noviembre, con Fabián.
- Sesión [«Best tips for your first hackathon»](https://www.youtube.com/watch?v=S9LyP7V82UQ), jueves 26 de noviembre, de Dev3pack.
- Clases [«Basics of Blockchain»](https://www.youtube.com/watch?v=gZLBW0FJbHk) y [«Deployment + Tips & Tricks»](https://www.youtube.com/watch?v=ZWlm8H3htKc), en español, del Solana Rust Bootcamp de Dev3pack.
- Prueba completa de NoahAI hecha por ChileDAO el lunes 23 de noviembre.
- Prueba de la ruta gratis hecha por ChileDAO el jueves 26 de noviembre: un programa escrito por DeepSeek, compilado y desplegado en devnet con Solana Playground.
- Correo de Dev3pack sobre los créditos de NoahAI, del jueves 26 de noviembre: créditos agotados y 30 % de descuento.

## Licencia

Este contenido está bajo [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.es): puedes copiarlo y adaptarlo citando a ChileDAO.
