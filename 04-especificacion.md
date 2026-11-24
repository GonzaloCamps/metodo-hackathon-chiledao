# 4. Alcance y especificación

## Tú planificas, NoahAI ejecuta

En la sesión del martes 24, Santiago lo explicó con dos roles: una arquitecta que diseña la casa y un equipo de construcción que la levanta. NoahAI es muy bueno construyendo, pero para pensar la idea, el nombre o el logo conviene otra IA, como ChatGPT, Claude o Codex, que no gasta tus créditos de NoahAI.

Su método tiene cuatro pasos:

1. **Prompt:** le cuentas la idea a tu IA de planificación.
2. **Especificación:** esa IA te ayuda a escribir un archivo con el plan completo.
3. **Código:** pegas la especificación en NoahAI y construye.
4. **Despliegue:** NoahAI publica el programa en devnet y la app.

Los pasos 1 y 2 los hace [00-instrucciones-para-tu-ia.md](00-instrucciones-para-tu-ia.md).

## Para cuidar tus créditos

- **Mitad del tiempo planificando y mitad ejecutando.**
- **Todo en los primeros 2 o 3 prompts.** Después NoahAI empieza a perder contexto.
- **La especificación en inglés**, porque gasta menos créditos. La interfaz puede quedar en español.
- **El modelo Core en vez de Ultra.** Ultra viene por defecto y es el de mayor costo.
- **La interfaz y el programa en la misma especificación**, para que calcen.
- **Un registro de cambios.** Santiago le pide a su IA que anote cada cambio en un archivo, como una bitácora, para saber qué cambió y por qué.
- **Si se te acaban los créditos,** tu código queda en GitHub: lo clonas y sigues con otra IA.

## Acotar a dos días

- **Un flujo principal**, de 3 a 5 pasos.
- **Una acción principal en Solana:** qué dato guarda el programa y qué acción permite.
- **Tu público:** ¿sabe de cripto? Si no sabe, la interfaz no usa jerga. Santiago armó su demo para gente que no sabe nada de cripto: solo «sube» o «baja».
- **Lo que queda fuera**, por escrito.
- **Los supuestos**, revisados uno por uno. Un supuesto equivocado hace que NoahAI construya lo que no era, y rehacerlo cuesta créditos.

## La especificación

Lleva estas secciones; el formato completo está en la etapa 6 de [00-instrucciones-para-tu-ia.md](00-instrucciones-para-tu-ia.md):

| Sección | Qué dice |
| --- | --- |
| Product vision | Qué es, en una frase |
| Target users | Para quién, y si sabe de cripto |
| Problem | El problema que resuelve |
| Main user flow | Los pasos del flujo principal |
| On-chain program | Qué cuentas y datos guarda el programa, qué instrucciones tiene y qué reglas y errores aplica |
| Screens | Las pantallas |
| Design | Idioma, colores y estilo |
| Confirmed decisions and assumptions | Lo que ya decidiste y los supuestos confirmados |
| Out of scope | Lo que no se construye |
| Answers to NoahAI design questions | Las respuestas a las preguntas de NoahAI |

## Las preguntas de NoahAI

Antes de construir, NoahAI hace cinco preguntas de diseño y alcance, y cambian según la idea. En la prueba que hizo ChileDAO el lunes 23, con una app de contador, fueron:

1. Qué tema de color prefieres.
2. Qué estilo buscas.
3. Una decisión propia de la app: si el contador era uno para todos o uno por wallet.
4. Qué funciones extra quieres.
5. Referencias, colores de marca o notas adicionales. Dice «opcional», pero no deja seguir sin escribir algo.

Si la especificación ya trae las respuestas, solo las copias.

## El segundo prompt

Decide de antemano el único cambio que le pedirás a NoahAI después de la primera versión. Pedidos sueltos, uno detrás de otro, gastan créditos y contexto.

## Resultado de esta etapa

La especificación en un bloque, lista para pegar en NoahAI, y el segundo prompt. Sigue con [05-construir-y-entregar.md](05-construir-y-entregar.md). Para ver un ejemplo completo, abre [ejemplos/ruta-del-hacker.md](ejemplos/ruta-del-hacker.md).
