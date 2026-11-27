# 5. Construir y entregar

## Si construyes con tu IA

Esta es la segunda conversación del método. Abre una conversación nueva en tu IA y pega tres cosas: este prompt, tu especificación y este archivo completo, que puedes copiar desde su [versión en texto plano](https://raw.githubusercontent.com/GonzaloCamps/metodo-hackathon-chiledao/main/05-construir-y-entregar.md).

```
Voy a construir mi proyecto para la Dev3pack Global Hackathon sobre Solana. Abajo van mi especificación y el paso 5 del Método Hackathon ChileDAO. Guíame con lo que dice ese archivo, sin saltarte pasos ni cambiarlos por otros que conozcas. Primero pregúntame por cuál ruta voy, la gratis o NoahAI, y qué tengo listo. Dame un paso a la vez y espera a que te cuente cómo me fue. Si te pego un error, corrígelo y devuélveme el archivo completo. Si después de un par de intentos no avanzo por la ruta gratis, recomiéndame pasar a NoahAI con la misma especificación.

MI ESPECIFICACIÓN:
[pega aquí]

PASO 5 DEL MÉTODO:
[pega aquí este archivo completo]
```

Si tu IA avisa que el mensaje es muy largo, envía primero el prompt con la especificación y después el archivo, en un segundo mensaje.

## Lo que cambió el jueves 26

Dev3pack avisó por correo que los créditos de NoahAI para la hackathon se agotaron. Cerró el formulario de créditos y, en su lugar, anunció un 30 % de descuento para el viernes 27, sin cupón: el plan Starter baja de USD 10 a USD 7, y con eso alcanza para varias iteraciones. Nada de esto afecta tu inscripción, y no hace falta pagar: también se puede construir gratis, con la ruta que está en este mismo archivo. Si llenaste el formulario a tiempo, revisa tu cuenta de NoahAI antes de pagar: si te asignaron créditos, aparecen ahí. La organización dijo que se entregan por orden de llegada y que no alcanzan para todas las personas.

## Cuál ruta usar

| | Ruta gratis | Ruta NoahAI |
| --- | --- | --- |
| Qué IA usas | Una IA gratuita de uso general: DeepSeek, ChatGPT o Claude | NoahAI, una IA hecha para construir apps en Solana |
| Cuánto cuesta | Nada | USD 7 con el descuento del viernes 27 (USD 10 sin él), o tus créditos si alcanzaste a recibirlos. Alcanza para varias iteraciones |
| Qué hace la IA por ti | Escribe el código. Tú lo compilas, lo despliegas y lo publicas, siguiendo los pasos de este archivo | Escribe el programa y la interfaz, despliega en devnet y publica la app |
| Qué tan fácil es | Tiene más pasos a mano | Es más fácil: casi todo sale de tu especificación |
| Qué tan probada está | El programa, probado por ChileDAO el jueves 26. La interfaz, solo a medias | Probada completa por ChileDAO el lunes 23 y repetida después con otras apps |
| Cuándo conviene | Para partir sin pagar | Si no logras avanzar por la ruta gratis, o si prefieres el camino más corto |

Las dos parten igual: con tu especificación, hecha con [00-instrucciones-para-tu-ia.md](00-instrucciones-para-tu-ia.md). Todo se hace en devnet, con SOL de prueba: no uses dinero real.

Nuestra recomendación: parte por la ruta gratis. Si te trabas y no logras avanzar, pasa a NoahAI con la misma especificación: es más fácil, y por USD 7, con el descuento del viernes 27, tienes para varias iteraciones. La entrega cierra el domingo 29 a las 04:00, así que organízate para terminar el sábado en la noche.

## Lo que pidió la organización el jueves 26

En su sesión de consejos para la hackathon ([video](https://www.youtube.com/watch?v=S9LyP7V82UQ), en inglés), la organizadora repasó lo que más pesa al evaluar. Sirve para las dos rutas:

- **Una app real, no una landing.** Tiene que ser un producto donde la persona usuaria hace algo. Entregar solo una landing, dijo, es eliminatorio.
- **Tres cosas para que puedan evaluarte:** el video de máximo 3 minutos, el repositorio público en GitHub y la app publicada en Vercel, Netlify o algo similar.
- **El repositorio, en público.** Si queda privado no lo pueden revisar, y el proyecto queda eliminado.
- **Un README completo.** Lo lee la IA del jurado y le da el contexto técnico para revisar tu repositorio. Suma un diagrama de cómo funciona la app, hecho por ejemplo en [Excalidraw](https://excalidraw.com) y pegado como captura: ayuda aunque no todo funcione, porque muestra qué quisiste construir.
- **Evalúan jueces locales y una IA.** La IA revisa a fondo la integración técnica, para comprobar que el proyecto hace lo que dice, y pone un puntaje con fortalezas y mejoras. Al final, cada proyecto recibe su informe.
- **Un solo foco.** Puedes postular a varios tracks, pero recomendó concentrarse en una línea. Cada partner tiene sus requisitos: respétalos.
- **Muéstralo en público.** Cuando envíes, y de nuevo con el resultado final, publica tu proyecto y etiqueta a @dev3pack, @solana y @TryNoahAI.

## Antes de construir

- **Inscripción:** en la [plataforma de Dev3pack](https://app.dev3pack.xyz/s/CHILE) y, si vas a la Build Station, en el [Luma de ChileDAO](https://luma.com/ovbwi0fj), con el mismo correo. Puedes inscribirte hasta el mismo viernes.
- **Cuentas:** GitHub, Vercel (el plan gratis alcanza y la cuenta se crea con GitHub) y una IA gratuita, como DeepSeek, ChatGPT o Claude. NoahAI (entras con Google en [trynoah.ai](https://trynoah.ai)) solo si vas por esa ruta.
- **Phantom en modo de prueba:** instala la extensión y, en Configuración, entra a Developer Settings, activa Testnet Mode y elige Solana Devnet. Si ya usas Phantom con fondos reales, crea una cuenta aparte para la hackathon: la organización recomienda no desarrollar con tu wallet personal.
- **SOL de prueba:** se pide en [faucet.solana.com](https://faucet.solana.com), entrando con GitHub: sin GitHub permite dos solicitudes cada 8 horas, y con GitHub el límite sube. Pídelo apenas puedas: la organización advirtió que durante la hackathon todos lo piden a la vez y el faucet se satura. Para usar una app basta 1 SOL en Phantom. Si vas por la ruta gratis, necesitas además 5 SOL para la billetera de Solana Playground: el paso 3 de esa ruta dice cómo pedirlos.

## Ruta gratis

Para enviar la entrega son obligatorias tres cosas: la dirección de tu programa en devnet, un repositorio público y un video de menos de 3 minutos. Ninguna exige una interfaz. Por eso esta ruta tiene dos partes: una meta mínima, que ya te deja enviar, y después la interfaz.

No dejes la interfaz como un extra. La organización cuenta la app publicada entre las tres cosas clave para evaluar un proyecto, y el premio principal pide el link a la demo en vivo. Sin app publicada el formulario se puede enviar, pero el jurado tiene menos que evaluar y quedas fuera del premio principal.

ChileDAO la probó el jueves 26 con una app de votación. El programa lo escribió DeepSeek en su versión gratuita, compiló en Solana Playground en 7 segundos y quedó desplegado en devnet en 7 minutos.

Si quieres ver un despliegue explicado en español, está la clase [Deployment + Tips & Tricks](https://www.youtube.com/watch?v=ZWlm8H3htKc) del Solana Rust Bootcamp de Dev3pack.

### Meta mínima: programa, repositorio y video

1. **Pídele el programa a tu IA.** En tu conversación de construir, o en la misma donde hiciste la especificación, pega esto:

   ```
   Con la especificación de arriba, escribe solo el programa en Anchor (Rust), en un único archivo lib.rs, para compilarlo y desplegarlo en Solana Playground (beta.solpg.io). Usa la versión de Anchor que trae Solana Playground y deja declare_id!("11111111111111111111111111111111"): Playground lo reemplaza al compilar. No uses init_if_needed, Token-2022 ni eventos. Calcula bien el espacio de cada cuenta: 8 bytes del discriminador más los campos. No escribas la interfaz todavía. Después dime en qué orden llamar las instrucciones para probar el programa, y con qué valores.
   ```

   Mientras más simple el programa, mejor: cada cuenta y cada instrucción de más es otra cosa que puede fallar.

2. **Abre Solana Playground** en [beta.solpg.io](https://beta.solpg.io) y crea su billetera con el botón «Not connected», abajo a la izquierda. Te ofrece guardar el archivo de la billetera: guárdalo, porque la billetera vive en ese navegador. No lo compartas ni lo subas al repositorio.
3. **Dale SOL de prueba a esa billetera.** Su dirección aparece en la barra de abajo. Cópiala, entra a [faucet.solana.com](https://faucet.solana.com) con GitHub y pide 5 SOL para esa dirección. Playground intenta pedir SOL por su cuenta y muestra un error 410, porque ese faucet está cerrado: no importa.
4. **Crea el proyecto y pega el programa.** Con «Create a new project» eliges Anchor, y reemplazas el contenido de `src/lib.rs` por el que te dio tu IA.
5. **Compila con Build,** en la pestaña Build & Deploy. Si sale un error, cópialo completo, pégaselo a tu IA, pídele el archivo corregido entero y vuelve a compilar.
6. **Despliega con Deploy.** Tarda: en nuestra prueba fueron 7 minutos, con avisos de «Reached rate-limits» y «transactions not confirmed, retrying». Es normal, porque el servidor público de devnet limita las solicitudes. No cierres la pestaña hasta leer «Deployment successful». Nuestro programa usó cerca de 1,6 SOL de prueba.
7. **Anota la dirección del programa y baja el IDL.** La dirección está en «Program ID», en la misma pestaña, y el IDL se baja con Export, en la sección IDL. Comprueba la dirección en [explorer.solana.com](https://explorer.solana.com), eligiendo Devnet: tiene que decir «Program Account» y «Executable: Yes».
8. **Prueba el programa sin interfaz.** Hay dos formas, y ninguna la hemos probado todavía nosotros:
   - la pestaña Test de Playground, en el panel izquierdo, para llamar las instrucciones del programa ya desplegado, en el orden que te dio tu IA;
   - pedirle a tu IA un archivo de pruebas para Playground (`tests/anchor.test.ts`) y ejecutarlo escribiendo `test` en la terminal de Playground, como indica la documentación de Anchor.

   Cada llamada queda como una transacción que puedes abrir en el explorador.
9. **Sube el código a un repositorio público.** En GitHub creas un repositorio público y, con «Add file» y «Create new file», pegas el programa con el nombre `programa/lib.rs` (al escribir la barra, GitHub crea la carpeta). Sube también el IDL, como `programa/idl.json`, y un README que diga qué problema resuelve, cuál es la dirección del programa en devnet y cómo probarlo. No hace falta instalar nada. Si tu programa tiene una instrucción que deja fijo al administrador, como `initialize`, llámala tú antes de publicar la dirección: quien la llame primero queda como administrador.
10. **Graba el video,** de menos de 3 minutos: el problema, el programa en Playground, una llamada a una instrucción y la transacción en el explorador.

Con eso ya puedes enviar la entrega. Lo que no tienes es el link a la demo en vivo: lo pide el premio principal y es una de las tres cosas que la organización considera clave para evaluar. Envía igual, para asegurar la entrega, y sigue con la interfaz: puedes editar el formulario hasta el cierre.

### Después: la interfaz y la demo en vivo

Esta parte no está probada de punta a punta. En nuestra prueba hubo que corregir varios errores de la IA gratuita: la app llegó a correr en el computador y a conectar la billetera, pero con fallas. Parte cuando tengas lista la meta mínima. Si después de un par de intentos no logras avanzar, pasa a NoahAI con la misma especificación: por USD 7, con el descuento del viernes 27, tienes para varias iteraciones.

1. **Instala Node** en su versión LTS, desde [nodejs.org](https://nodejs.org). Si usas un computador donde no puedes instalar nada, GitHub Codespaces trae Node en el navegador; no lo hemos probado.
2. **Crea el proyecto** con `npm create vite@latest`, eligiendo React y TypeScript.
3. **Pídele la interfaz a tu IA,** pegando la dirección del programa y el IDL:

   ```
   Con la especificación, la dirección del programa desplegado en devnet y su IDL, escribe la interfaz como una app Vite + React + TypeScript. Usa el wallet adapter de Solana con Phantom en devnet, y @coral-xyz/anchor fijado en la versión 0.29.0 exacta en package.json, sin el símbolo ^, porque el IDL viene en el formato antiguo de Anchor. Envía los números de tipo u64 como BN. Usa la menor cantidad de archivos posible y entrégame cada archivo completo con su ruta, más un README con qué hace la app, cómo probarla y la dirección del programa.

   Dirección del programa: [pega aquí]
   IDL: [pega aquí]
   ```

   En nuestra prueba, Playground entregó el IDL en el formato antiguo de Anchor: por eso el pedido fija la versión 0.29.0. DeepSeek entrega cada archivo por separado, y hay que guardarlo con su nombre y en su carpeta. En nuestra prueba, DeepSeek escribió los archivos y ChatGPT los empaquetó en un ZIP. Si una IA te arma el ZIP, revisa que no haya cortado ningún archivo: a nosotros nos llegó el programa cortado a la mitad.
4. **Pruébala en tu computador** con `npm install` y `npm run dev`. Cuando salga un error, pégaselo a tu IA y reemplaza el archivo completo. Cuenta con varias vueltas. Al revisar la interfaz que escribió la IA en nuestra prueba encontramos dos errores, y conviene mirarlos primero:
   - `package.json` pedía Anchor 0.30, que no lee el IDL del formato antiguo: tiene que decir `"@coral-xyz/anchor": "0.29.0"`. Si lo cambias, borra `node_modules` y `package-lock.json` y corre `npm install` de nuevo.
   - Enviaba números comunes donde el programa espera `u64`: Anchor los necesita como `BN`, por ejemplo `new BN(10)`.
5. **Súbela al mismo repositorio.** Arrastra todos los archivos y carpetas menos `node_modules`: la web de GitHub no acepta más de 100 archivos por subida. Si sabes usar git, usa git.
6. **Publícala en Vercel:** importas el repositorio y presionas Deploy. Queda un link del tipo nombre.vercel.app. Si la construcción falla, Vercel muestra el error en su registro: corriges el archivo en GitHub y Vercel vuelve a desplegar.

## Ruta NoahAI

Es la ruta más fácil: NoahAI construye el programa y la interfaz a partir de tu especificación. Sirve si tienes créditos o si tu equipo paga el plan Starter, y basta una cuenta por equipo. Si no quieres pagar, la ruta gratis de más arriba también llega a una entrega.

- **Precio:** el plan Starter cuesta USD 10. Con el 30 % de descuento del viernes 27 queda en USD 7, y alcanza para varias iteraciones si usas el modelo Core.
- **Descuento:** rige en toda la plataforma de NoahAI, sin cupón, desde las 08:00 de Chile.
- **Es una suscripción** que se renueva cada mes: si no la vas a seguir usando, cancélala.

La sesión donde Santiago mostró este flujo es [Vibecode your first app on Solana](https://www.youtube.com/watch?v=cMhjoZOhM0Q), en inglés.

Este es el recorrido que ChileDAO probó completo el lunes 23. Una app simple tomó unos 25 minutos y usó cerca del 11 % de los créditos de un plan de USD 10. El martes 24, la Ruta del Hacker de los [ejemplos](ejemplos/ruta-del-hacker.md), con su especificación completa y el modelo Core, quedó con el programa en devnet en unos 5 minutos.

1. **Cambia el modelo de Ultra a Core** antes del primer prompt. Si la página se recarga, vuelve a Ultra: revísalo antes de cada prompt.
2. **Elige el modo Full Stack Dapp y pega tu especificación.**
3. **Responde las preguntas de diseño y alcance**, copiando las respuestas de tu especificación. Si tu especificación ya trae esas respuestas, NoahAI puede saltarse las preguntas y pasar directo a su plan de trabajo.
4. **Deja que construya.** NoahAI escribe el programa en Rust con Anchor, lo prueba y lo despliega en devnet. En nuestra prueba lo desplegó sin pedir SOL. En la sesión del martes 24, en cambio, el despliegue falló por falta de fondos y hubo que pedir SOL de prueba en el faucet para la dirección de despliegue que muestra NoahAI.
5. **Anota la dirección del programa:** está en Publish, pestaña Smart Contract. NoahAI guarda la llave que administra el programa y permite descargarla: no la compartas ni la subas al repositorio.
6. **Conecta GitHub** desde el ícono de la barra superior del proyecto. NoahAI crea el repositorio y sube cada cambio, pero lo crea privado y sin README.
7. **Publica la demo en vivo:** en Publish, pestaña Web App, elige Vercel (puede venir marcado Netlify) y conecta tu cuenta. Al autorizar, elige «All Projects». Presiona Deploy y queda un link del tipo nombre.vercel.app.
8. **Prueba la app con Phantom en modo de prueba.** Cada uso gasta muy poco SOL de prueba, cerca de 0,001. En modo de prueba el historial de Phantom aparece vacío: para ver una transacción, usa el enlace al explorador que trae la app.

## Problemas frecuentes

### En Solana Playground

| Síntoma | Causa | Qué hacer |
| --- | --- | --- |
| Aparece un error 410 al pedir SOL | Playground intenta pedir SOL por su cuenta, y ese faucet está cerrado | Pedir SOL en faucet.solana.com para la dirección de la billetera de Playground |
| El Build falla | Un error en el código que escribió la IA | Pegarle el error completo a la IA y reemplazar el archivo entero |
| El Deploy muestra «Reached rate-limits» o «transactions not confirmed, retrying» | El servidor público de devnet limita las solicitudes | Esperar sin cerrar la pestaña; en nuestra prueba terminó en 7 minutos |
| La dirección del programa no aparece como programa en el explorador | El despliegue no ha terminado, o el explorador no está en Devnet | Esperar «Deployment successful» y elegir Devnet en el explorador |
| En otro computador o navegador no están el proyecto ni la billetera | Playground los guarda en el navegador | Trabajar siempre en el mismo navegador y guardar el archivo de la billetera |

### En NoahAI y al probar la app

| Síntoma | Causa | Qué hacer |
| --- | --- | --- |
| NoahAI no deja enviar las preguntas | La última dice «opcional», pero exige texto | Escribir algo breve |
| Los créditos se gastan rápido | El modelo Ultra viene por defecto, es el más caro y vuelve si la página se recarga | Revisar que diga Core antes de cada prompt |
| NoahAI se queda pegado | Una falla de la plataforma | Volver a enviar el prompt |
| Aparece una página de verificación de seguridad | La protección del sitio, que a veces salta al navegar o recargar | Esperar unos segundos; si pide marcar una casilla, marcarla |
| Al desplegar, avisa que faltan fondos | La dirección de despliegue no tiene SOL de prueba | Pedir SOL en el faucet para esa dirección |
| No encuentras la dirección del programa | Está en otra pestaña | Publish, pestaña Smart Contract |
| El plan del proyecto se queda a medias, por ejemplo en «1 of 3 Done» | El indicador no se actualiza, aunque el código esté listo | Revisar el código y Publish, no el indicador |
| Al conectar Vercel, pide elegir un proyecto y no aparece ninguno | El proyecto en Vercel lo crea NoahAI al publicar | Elegir «All Projects» |
| El repositorio no se ve desde otra cuenta | NoahAI lo crea privado | En GitHub, Settings, sección Danger Zone, pasarlo a público |
| Phantom no muestra la transacción | En modo de prueba el historial aparece vacío | Usar el enlace al explorador que trae la app |
| El faucet no entrega SOL | Límite de dos solicitudes cada 8 horas | Entrar con GitHub, que sube el límite, o probar la app con la wallet de otra persona del equipo que tenga SOL |
| NoahAI ofrece una auditoría de seguridad (FYEO) | Es un servicio que se paga con créditos de NoahAI | No hace falta para entregar |

## Qué necesitas para entregar

Obligatorio para enviar el formulario:

- **La dirección de tu programa.** Sirve una de devnet. Sin dirección no se puede enviar.
- **Un repositorio público en GitHub.** Antes de hacerlo público, revisa que no tenga claves propias ni la llave del programa. Si queda privado, el jurado no puede revisarlo y el proyecto queda eliminado.
- **Un video de menos de 3 minutos** que muestre el producto funcionando, con un link público. Uno más largo queda fuera de premios; en el track de Pollar el máximo es de 2 minutos.

Para optar al premio principal, además:

- **Un programa propio en Rust,** desplegado al menos en devnet.
- **Un README** con qué problema resuelve el proyecto, cómo instalarlo y probarlo, y las direcciones del programa. Hazlo completo, porque lo lee también la IA del jurado, y suma si puedes un diagrama de cómo funciona la app. Si partiste con código propio anterior, cuenta qué existía y qué hiciste durante la hackathon. NoahAI no crea el README: tienes que agregarlo tú.
- **El link a la demo en vivo,** publicada en Vercel o Netlify, para que el jurado pruebe el proyecto. Tiene que ser una app que se usa, no una landing.

El formulario pide también capturas de pantalla, y el nombre, la frase corta y la descripción del proyecto. La organizadora mencionó además logo y banner: tenlos a mano.

## El formulario

Está en la pestaña Project del panel y tiene 5 pasos: Project, Images, Links & video, Team, y Review & submit. Puedes guardarlo como borrador y editar todo hasta el cierre. Si participas desde la Build Station, en el campo Hub elige «Dev3pack Build Station (Santiago)».

Por cada track de partner que marques, el formulario pide explicar cómo lo integraste. Sé específico e indica el archivo donde está esa integración: le facilita el trabajo al jurado.

## Fechas, en hora de Chile

| Cuándo | Qué pasa |
| --- | --- |
| Viernes 27, 12:00 a 13:00 | Kickoff global, online |
| Viernes 27, 13:00 a 18:00 | Build Station en la UDP, presencial y opcional |
| Sábado 28, 10:00 a 12:00 | Sesión online de feedback de proyectos |
| Domingo 29, 04:00 | Cierre de entregas |

La entrega cierra en la madrugada del sábado al domingo: organízate para terminar el sábado en la noche. El panel muestra la hora de cierre en tu zona horaria. Antes de enviar, abre cada link en una ventana privada para comprobar que es público.
