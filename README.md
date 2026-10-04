# Perfil UCP de OfertasChileBot

Este repositorio publica un solo archivo: [`perfil.json`](perfil.json), el perfil de agente que exige el
[Universal Commerce Protocol](https://ucp.dev) para consultar el catálogo de una tienda por su endpoint MCP.

**Qué es el bot.** OfertasChileBot vigila los precios de tiendas chilenas y publica las buenas ofertas y los
errores de precio en el canal de Telegram [@OfertitasHumildes](https://t.me/OfertitasHumildes).

**Qué declara el perfil.** Solo lectura de catálogo (`catalog.search` y `catalog.lookup`). No declara carrito ni
pago: el bot no compra, no agrega nada a un carrito y nunca completa un checkout. Tampoco declara medios de pago.

**Cómo se comporta el bot con las tiendas.** Respeta el `robots.txt` de cada sitio, se identifica con su propio
User-Agent, espera entre consultas y, si una tienda pide bajar el ritmo, deja de consultarla un rato. Si una tienda
bloquea al bot, no se intenta esquivar el bloqueo.

Contacto: por el canal de Telegram.
