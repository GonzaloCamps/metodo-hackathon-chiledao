# 2. Validar

## ¿Ya existe?

**Si usas un agente de IA** (Claude Code, Codex u otro), instala [Colosseum Copilot](https://colosseum.com/copilot). Es una skill que conoce las entregas de hackathones anteriores de Solana y del ecosistema; las instrucciones para instalarla están en su página. En la [sesión del lunes 23](https://www.youtube.com/watch?v=yM6HUVMjxdI) la recomendaron para todas las personas, con preguntas como:

- «¿Alguien construyó una forma de que los fans financien a artistas?»
- «¿Qué le falta a mi idea frente a lo que ya existe?»

**Si no usas un agente,** busca a mano:

- en los [ganadores de hackathones de Solana](https://superteam.fun/build/past-hackathon-winners);
- en la [galería de mayo de 2026](https://app.dev3pack.xyz/hackathon/projects?season=may-2026), donde cada ficha trae demo, repositorio y video;
- en los [proyectos del Colosseum Agent Hackathon](https://colosseum.com/agent-hackathon/projects), si tu idea usa agentes;
- en el [mapa de los 30 finalistas de mayo](referencias/ganadores-mayo-2026.md), ordenados por tipo de proyecto.

Que exista algo parecido no mata tu idea. Busca qué harías distinto: otro usuario, otro lugar u otra parte del problema.

## ¿Por qué ahora?

En la sesión mostraron ideas del ecosistema presentadas con tres preguntas: qué construir, por qué ahora y por qué en Solana. Un ejemplo: pagar suscripciones con stablecoins, porque cada vez más negocios las están adoptando. Las [Requests for Startups de Solana](referencias/requests-for-startups.md) responden esas preguntas para once ideas: sirven de modelo para responderlas sobre la tuya.

Pregúntate qué cambió para que tu idea tenga sentido hoy y no hace tres años.

## ¿Por qué en Solana?

El track principal pide un programa propio en Rust, así que la blockchain tiene que hacer un trabajo real.

- ¿Qué dato o acción tiene que quedar en un registro público que nadie puede alterar?
- ¿Hay pagos, propiedad o reglas que se cumplen solas?
- Si sacas la blockchain, ¿la app queda igual? Si la respuesta es sí, Solana está de adorno.

El jueves 26, la organizadora de la hackathon lo repitió: construir sobre la blockchain es más que aceptar pagos en cripto.

Dos ejemplos de la sesión:

- Llevar a la cadena un activo del mundo real, como una carta coleccionable, para que quien la compre vea su historial y sepa si es legítima.
- Un panel único para quien apuesta en varios mercados de predicción y quiere ver todas sus posiciones juntas.

### Qué hace distinta a Solana

Para responder con datos, sirve saber en qué se diferencia Solana de las otras blockchains que más vas a oír:

| | Bitcoin | Ethereum (red principal) | Solana |
| --- | --- | --- | --- |
| Para qué nació | Guardar y mover valor | Ser la primera plataforma de programas, o contratos inteligentes | Correr apps a gran escala, rápido y barato |
| Un bloque nuevo cada | 10 minutos, aproximadamente | 12 segundos | 0,2 segundos, aproximadamente |
| Cuándo una transacción queda firme | Cerca de una hora, por convención | Cerca de 13 minutos | Menos de un segundo |
| Cuánto cuesta una transacción | Varía con la demanda | Varía con la demanda | Base fija de 0,000005 SOL por firma: una fracción de centavo de dólar |
| Cómo crece | Con redes aparte, encima de la principal | Con redes de segunda capa (L2), encima de la principal | En una sola red |
| En qué se programa | Casi no admite programas | Solidity | Rust |

Lo que eso significa cuando construyes una app:

- **Responde como una app normal.** Con un bloque cada 0,2 segundos y transacciones que quedan firmes en menos de un segundo, quien usa tu app no espera. Esto último es nuevo: llegó con la actualización Alpenglow, en octubre de 2026.
- **Cada acción cuesta casi nada.** La comisión es tan baja que puedes registrar, premiar o cobrar montos muy chicos muchas veces, sin que el costo se coma el valor. Por eso en Solana funcionan los micropagos y los pagos entre agentes de IA.
- **Todo vive en una sola red.** Ethereum bajó sus costos sumando muchas redes de segunda capa, pero los usuarios y los fondos quedan repartidos entre ellas. En Solana todos los programas y tokens comparten el mismo estado: tu programa puede usar otro en la misma transacción, sin puentes.
- **Procesa en paralelo.** Cada transacción declara qué cuentas va a tocar, y las que no se cruzan se ejecutan al mismo tiempo. La red principal de Ethereum, en cambio, las ejecuta de a una. Así Solana aguanta más carga.
- **Tiene herramientas para partir rápido.** Con Anchor, Solana Playground y la red de prueba, que entrega SOL gratis, puedes escribir, desplegar y probar un programa desde el navegador. Es lo que usa este método en el paso 5.

Lo que conviene saber, para elegir con los ojos abiertos:

- **Ethereum es más antigua y concentra más valor.** Tiene muchos más validadores y cerca de la mitad del dinero de las finanzas descentralizadas. Cuando lo único que importa es la máxima seguridad, muchos proyectos la prefieren.
- **Validar en Solana exige equipos potentes,** así que la red tiene menos validadores. Es la crítica más frecuente a su descentralización.
- **Solana se cayó varias veces entre 2021 y comienzos de 2024.** Desde febrero de 2024 no ha tenido una caída completa.
- **Rust y el modelo de cuentas cuestan más que Solidity al principio.** Por eso este método se apoya en una IA y en Anchor.

En resumen: para una app que la gente usa todos los días, con muchas acciones chicas, Solana es una de las opciones más fuertes. Si tu idea no aprovecha ninguna de estas ventajas, vuelve a las tres preguntas de arriba.

Datos revisados el 27 de noviembre de 2026. Las fuentes están al final del [README](README.md#fuentes).

## Resultado de esta etapa

Lo que existe, tu diferencia y por qué Solana, en tres líneas. Sigue con [03-pauta.md](03-pauta.md).
