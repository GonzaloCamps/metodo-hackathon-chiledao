# 1. La idea

## Parte de tu contexto

En la sesión del lunes 23, Deepesh y Solene insistieron en lo mismo: no elijas una idea al azar.

- **Busca donde tienes red, experiencia o pasión.** Si construyes algo de entretenimiento sin conocer a nadie en ese mundo, te va a costar hacer lo correcto para las personas correctas.
- **Mira los problemas de tu día a día y de tu entorno.** En Argentina muchos equipos construyen soluciones de pago, porque la inflación les toca de cerca.
- **Construye algo que tú usarías.** Si tú no lo usarías, cuesta que otras personas lo usen.
- **No copies otro proyecto.** Inspírate, pero el problema tiene que ser el tuyo.

El ejemplo que mostraron: un estudiante que venía de la comedia armó un mercado de predicciones en vivo, donde se apuesta sobre casi cualquier cosa, y pasó los 8 mil usuarios. Le fue bien porque construyó lo que conocía, para la red que ya tenía.

## Lo que sumó la organizadora el jueves 26

En su sesión de consejos para la hackathon ([video](https://www.youtube.com/watch?v=S9LyP7V82UQ), en inglés) agregó:

- **Toda app necesita usuarios o liquidez.** Elige un área donde tengas llegada: tu oficio, tu país o tu comunidad. Así tu caso de uso es concreto y no el mismo de todos.
- **Si no tienes idea,** parte de una app que usas todos los días y piensa qué le suma la blockchain. Que funcione bien en el celular.
- **Mira otras redes.** Busca apps que funcionan en otros ecosistemas y todavía no existen en Solana.
- **Si es DeFi,** revisa en [DeFi Llama](https://defillama.com) qué protocolos mueven liquidez real en cada red.
- **Los ganadores anteriores son referencia, no molde.** Ganaron porque consiguieron usuarios e impacto en su área, no solo por ser novedosos.
- **Un solo foco.** Puedes postular a varios tracks, pero conviene concentrarse en una línea.

## Preguntas para partir

- ¿Qué problema vives tú, o alguien cercano, con frecuencia?
- ¿Quién lo tiene? Piensa en una persona concreta.
- ¿Cómo lo resuelve hoy? ¿Qué le molesta de esa solución?
- ¿Usarías tu app? ¿Quiénes más la usarían?
- ¿Qué parte del problema tiene que ver con dinero, propiedad, registros o confianza? Ahí suele entrar Solana.

## Dónde buscar inspiración

| Fuente | Qué tiene |
| --- | --- |
| [Colosseum Copilot](https://colosseum.com/copilot) | Compara tu idea con más de 11.000 entregas de hackathones. Se instala como skill en tu agente de IA |
| [Proyectos del Colosseum Agent Hackathon](https://colosseum.com/agent-hackathon/projects) | Agentes de IA ya construidos |
| [Superteam Build, ideas](https://superteam.fun/build/ideas) y [SendAI Ideas](https://ideas.sendai.fun/) | Ideas y prompts pensados para hackathon |
| [Ganadores de hackathones de Solana](https://superteam.fun/build/past-hackathon-winners) | Proyectos que ganaron |
| [Galería de mayo de 2026](https://app.dev3pack.xyz/hackathon/projects?season=may-2026) | Los 386 proyectos públicos de la edición anterior, con demo, repositorio y video |
| [Requests for Startups de Solana](https://solana.com/es/request-for-startups) | Once productos que el ecosistema de Solana quiere ver construidos, cada uno con por qué ahora y por dónde empezar. Resumen en [referencias/requests-for-startups.md](referencias/requests-for-startups.md) |
| Pestaña Prizes del panel de Dev3pack | Cada track trae su descripción, requisitos y recursos |

Inspirarse no es copiar: úsalas para ver qué existe y qué falta.

## Lo que ganó en mayo de 2026

La edición de mayo tuvo 382 proyectos de 84 países y 30 finalistas, y Chile tuvo su sede en la USACH. El mapa completo, con los 30 finalistas, los ganadores por track y los proyectos chilenos, está en [referencias/ganadores-mayo-2026.md](referencias/ganadores-mayo-2026.md). Lo que más se repitió:

- **Agentes de IA con pagos y seguridad:** 9 de los 30 finalistas.
- **Contexto local:** 5, como Tropico, una wallet para venezolanos, y CredIA, un score financiero para trabajadores informales de Ecuador.
- **Herencia cripto:** 4. AfterLife, de Costa Rica, ganó el primer lugar.
- **América Latina:** un tercio de los finalistas, 10 de 30.

En Chile, x402Warden ganó el bono global a la mejor implementación de x402. EduMint, Vaquita, FundBridge y CertiLink completan el ranking del país.

## Si tu idea usa pagos de agentes (x402)

En la sesión del miércoles 25, Fabián presentó [x402](https://x402.org), un protocolo abierto que convierte el código HTTP 402, «pago requerido», en un paso de pago: una API o una página cobra antes de responder, sin cuentas, claves ni checkout. Lo creó Coinbase y hoy lo administra la x402 Foundation, bajo la Linux Foundation.

Casos de uso que mostró:

- agentes de IA que pagan solos por datos, APIs o cómputo, consulta a consulta;
- APIs que cobran por consulta, sin planes ni facturas;
- herramientas MCP y modelos especializados que se pagan por uso;
- contenido con micropagos: imágenes, artículos o conjuntos de datos;
- otras ideas que citó de la guía de x402 de Solana: medir llamadas a un RPC, datos de mercado en tiempo real, lecturas de sensores, minutos de GPU, pagar para llegar a una bandeja de entrada y sesiones de juego.

Su diagnóstico: la infraestructura ya está lista y lo que faltan son apps útiles. Antes de elegir x402, ten en cuenta:

- el cobro lo hace un servidor aparte (en su demo, Node con Express) y se paga con USDC de devnet; no hemos probado si NoahAI arma ese servidor;
- igual necesitas un programa en Rust desplegado en devnet para entregar;
- todo se hace en devnet: no uses dinero real.

## Resultado de esta etapa

El problema y el usuario, en dos frases. Sigue con [02-validar.md](02-validar.md).
