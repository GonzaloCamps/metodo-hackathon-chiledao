# 5. Construir y entregar

## Antes del viernes

- **Inscripción:** en la [plataforma de Dev3pack](https://app.dev3pack.xyz/s/CHILE) y, si vas a la Build Station, en el [Luma de ChileDAO](https://luma.com/ovbwi0fj), con el mismo correo. Puedes inscribirte hasta el mismo viernes.
- **Cuentas:** NoahAI (entras con Google en [trynoah.ai](https://trynoah.ai)), GitHub y Vercel.
- **Créditos de NoahAI:** Dev3pack entrega USD 10 por participante y los carga directo en tu cuenta de NoahAI. El formulario está en el panel y en el grupo de Telegram de la hackathon. Usa el mismo correo con que te inscribiste en Dev3pack, porque con ese correo asignan los créditos. Envíalo una sola vez: quien lo envía muchas veces queda fuera.
- **Phantom en modo de prueba:** instala la extensión y, en Configuración, entra a Developer Settings, activa Testnet Mode y elige Solana Devnet.
- **SOL de prueba:** pide 1 SOL en [faucet.solana.com](https://faucet.solana.com), entrando con GitHub. Hazlo antes del viernes, porque el faucet limita las solicitudes.

## Construir en NoahAI

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
| El faucet no entrega SOL | Límite de solicitudes | Probar la app con la wallet de otra persona del equipo que tenga SOL |
| NoahAI ofrece una auditoría de seguridad (FYEO) | Es un servicio que se paga con créditos de NoahAI | No hace falta para entregar |

## Qué necesitas para entregar

- **Un programa en Rust desplegado en devnet y su dirección.** Sin dirección no se puede enviar el formulario.
- **Un repositorio público en GitHub.** Antes de hacerlo público, revisa que no tenga claves propias ni la llave del programa.
- **Un README** con qué problema resuelve el proyecto, cómo instalarlo y probarlo, y las direcciones de despliegue. Si partiste con código propio anterior, cuenta qué existía y qué hiciste durante la hackathon. NoahAI no crea el README: tienes que agregarlo tú.
- **La demo en vivo publicada**, en Vercel o Netlify, para que el jurado pruebe el proyecto.
- **Un video de menos de 3 minutos** que muestre el producto funcionando, con un link público. Uno más largo queda fuera de premios; en el track de Pollar el máximo es de 2 minutos.
- **Capturas de pantalla**, y el nombre, la frase corta y la descripción del proyecto.

## El formulario

Está en la pestaña Project del panel y tiene 5 pasos: Project, Images, Links & video, Team, y Review & submit. Puedes guardarlo como borrador y editar todo hasta el cierre. Si participas desde la Build Station, en el campo Hub elige «Dev3pack Build Station (Santiago)».

## Fechas, en hora de Chile

| Cuándo | Qué pasa |
| --- | --- |
| Viernes 27, 12:00 a 13:00 | Kickoff global, online |
| Viernes 27, 13:00 a 18:00 | Build Station en la UDP, presencial y opcional |
| Sábado 28, 10:00 a 12:00 | Sesión online de feedback de proyectos |
| Domingo 29, 04:00 | Cierre de entregas |

La entrega cierra en la madrugada del sábado al domingo: organízate para terminar el sábado en la noche. Antes de enviar, abre cada link en una ventana privada para comprobar que es público.
