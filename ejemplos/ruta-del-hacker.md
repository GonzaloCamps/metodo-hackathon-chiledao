# Ejemplo: Ruta del Hacker

Es el ejemplo que ChileDAO usa en la demo guiada de la Build Station de Santiago. Recorre el método completo, de la idea a la especificación, y además es una herramienta para la propia hackathon. No lo entregues como tu proyecto: el proyecto tiene que ser propio.

## 1. Contexto e idea

- **Contexto:** ChileDAO organiza la Build Station de Santiago y acompaña a los equipos chilenos durante la hackathon.
- **Problema:** al entregar, cada equipo tiene que declarar qué existía antes y qué hizo durante la hackathon, pero no tiene una forma simple de probar desde cuándo existía su idea. Además, entre la idea y la entrega hay varias etapas, y quienes acompañan a los equipos no saben en cuál va cada uno.
- **Usuario:** el equipo que participa usa la app. Mentoras, mentores y organizadores pueden mirar su ruta si el equipo les comparte su dirección.

## 2. Validación

Lo que existe:

- **El sello de tiempo es un uso conocido de la blockchain.** [OpenTimestamps](https://opentimestamps.org/) lo hace sobre Bitcoin desde 2016: guarda la huella de un documento, no el documento, y prueba que ese documento ya existía en una fecha.
- **En Solana hay proyectos que hacen algo parecido.** [SOLPRISM](https://colosseum.com/agent-hackathon/projects/axiom-protocol), del Colosseum Agent Hackathon, deja en la cadena la huella SHA-256 del razonamiento de un agente de IA antes de que actúe.
- **También hay proyectos de hackathon que sellan trabajo.** [Ghonsi Proof](https://chain.link/hack-26/projects/ghonsi-proof) registra con fecha los aportes de profesionales Web3, y [Filechain](https://devfolio.co/projects/filechain-6fd7) sella obras e ideas para probar desde cuándo existían.

La diferencia: ninguno de esos une el sello con la ruta de una hackathon, de la especificación a la entrega, ni está pensado para equipos que parten de cero.

Por qué en Solana: la fecha queda en un registro público que nadie puede cambiar después, ni siquiera el propio equipo. Una lista de tareas común se puede editar cuando quieras.

## 3. Pauta

| Criterio | Puntaje | Por qué |
| --- | --- | --- |
| Claridad | 4 | Junta dos cosas, el sello y la ruta, y toma una explicación corta |
| Impacto real | 3 | La declaración de qué existía antes la pide la hackathon, pero ningún equipo ha pedido esta app todavía |
| Ajuste entre el equipo y el problema | 5 | ChileDAO organiza y acompaña la hackathon en Chile |
| Por qué Solana | 4 | La fecha pública no se puede cambiar. Las etapas, en cambio, las declara el propio equipo y nadie las verifica |
| Diferencia | 3 | El sello ya existe en otros proyectos; la diferencia está en la ruta y en el público |
| Se puede probar | 4 | Se prueba sin fondos reales, pero el jurado necesita Phantom en devnet con SOL de prueba |
| Cabe en dos días | 4 | Un flujo y dos acciones en Solana: sellar y marcar etapas |

**Lectura:** ningún criterio queda en 2 o menos. Los más débiles son el impacto real y la diferencia. En un proyecto de verdad, el siguiente paso sería preguntarles a algunos equipos si la usarían.

**Propuesta de valor:** para los equipos de una hackathon, que tienen que demostrar qué hicieron durante el evento, Ruta del Hacker sella su especificación en Solana y registra con fecha cada etapa hasta la entrega, a diferencia de una lista de tareas común, que se puede editar después.

## 4. Alcance de dos días

- **Flujo principal:** conectar Phantom, pegar la especificación y el nombre del proyecto, sellar, marcar cada etapa cuando se cumple y ver la ruta con sus fechas.
- **Acciones en Solana:** crear la ruta con la huella de la especificación, y marcar una etapa.
- **Público:** muchos equipos parten de cero en cripto, así que la interfaz no usa jerga.
- **Queda fuera:** verificar que cada etapa se cumplió de verdad, una vista que liste las rutas de todos los equipos, guardar el texto de la especificación, NFT o tokens, y mainnet.
- **Supuestos confirmados:**
  - la huella se calcula en el navegador y el texto de la especificación nunca sale de ahí;
  - las etapas las declara el propio equipo;
  - las etapas se pueden marcar en cualquier orden, una vez cada una;
  - hay una ruta por wallet y el sello no se cambia después;
  - el sello prueba que la especificación ya existía en esa fecha. No prueba autoría ni es un registro de propiedad intelectual, y la app lo dice.

## 5. Especificación para NoahAI

```
# Ruta del Hacker - spec for NoahAI

Build this as a Full Stack Dapp on Solana devnet. Keep it simple: one main flow.

## Product vision
A hackathon route for teams: seal your project spec on Solana with a timestamp, then record each step until submission.

## Target users
Hackathon teams in Chile, many of them new to crypto, so the interface uses plain language and no blockchain jargon. Mentors and organizers can look at a team's route if the team shares its wallet address. There is no organizer screen in this version.

## Problem
Teams must declare what existed before the hackathon and what they built during it, and they have no simple way to prove since when their spec existed. Mentors don't know which step each team is on.

## Main user flow
1. The user opens the app and connects a Phantom wallet (devnet).
2. The user types the project name (max 50 characters) and pastes the project spec text.
3. The app computes the SHA-256 hash of the spec in the browser and creates the route on-chain with one click. The spec text never leaves the browser.
4. The user marks each step when it is done: "Programa en devnet", "Demo publicada", "README listo", "Video grabado", "Entrega enviada".
5. The app shows the route: the seal date and hash, each completed step with its date and time, and a Solana Explorer link (devnet) for each transaction.

## On-chain program (Rust, Anchor, devnet)
- Accounts and data: one Route account per wallet, a PDA with seeds ["route", owner]. It stores the owner, name (String, max 50 bytes), spec_hash ([u8; 32]), sealed_at (i64 unix timestamp), steps_done_at ([i64; 5], 0 means not done) and the bump.
- Instructions: create_route(name, spec_hash) creates the PDA for the signer and sets sealed_at from the Clock sysvar. complete_step(step_id: u8) sets steps_done_at[step_id] from the Clock sysvar.
- Rules and errors: only the owner can update their route. name must be 1 to 50 bytes (InvalidName). step_id must be between 0 and 4 (InvalidStep). Each step can be completed only once (StepAlreadyDone).

## Screens
- Home: connect wallet button and a one-line explanation.
- Seal: project name field, a large text area for the spec, a "Sellar mi idea" button, and two notes: "Tu especificación no se sube: solo se guarda su huella." and "El sello prueba que tu especificación ya existía en esta fecha. No es un registro de propiedad intelectual."
- Route: the seal with its date and hash, five steps with a "Marcar" button each (disabled once done), the date and time of each completed step, and explorer links.

## Design
- Interface language: Spanish (Chile)
- Color theme: dark
- Style: clean and simple, mobile first

## Confirmed decisions and assumptions
- The hash is computed in the browser with SHA-256. The spec text is never stored or sent.
- Steps are self-declared: the app does not verify them.
- Steps can be completed in any order, once each.
- One route per wallet. The seal cannot be changed after creation.
- The seal proves the spec existed at that date. It does not prove authorship.

## Out of scope
Verifying that a step was really done, an organizer view listing all routes, storing the spec text, NFTs or tokens, mainnet.

## Answers to NoahAI design questions
- Color theme: dark
- Style: clean and simple, mobile first
- Scope decision: one route per wallet, five fixed steps, any order
- Extra features: a Solana Explorer link for each transaction
- References or brand notes: none, keep it simple
```

## 6. Segundo prompt

```
On the Route screen, add a "Verificar" section: the user pastes a spec text, the app computes its SHA-256 hash in the browser and shows whether it matches the sealed hash. Do not change the program.
```

## Antes de pegarla en NoahAI

Cambia el modelo de Ultra a Core.
