# PRD — Propuesta Alianza Yafelin Espino Agencia × Jake Mate (2026)

## Problem statement original
"dame tu mejor version de esta propuesta que te comparto en html la idea es impactar al cliente" — Propuesta comercial de alianza estratégica (HTML) con tarifas Partner/US Retail 2026. Requisitos del usuario: HTML con botón de impresión a PDF, estilo "sorpréndeme", mantener logo Jake Mate y precios exactos, agregar nota de "todo es negociable".

## Arquitectura
- Entregable principal: `/app/frontend/public/alianza-yafelin-jakemate-2026.html` — HTML autónomo (single-file, CDN: Google Fonts, GSAP + ScrollTrigger, Lenis).
- Logo: `/app/frontend/public/jakemate-logo.png` (extraído del documento original, optimizado a 720px).
- `/` de la app React redirige a la propuesta (`App.js`).
- URL pública: {REACT_APP_BACKEND_URL}/alianza-yafelin-jakemate-2026.html

## Dirección de arte
"Cartel editorial cinético" — tinta #0C0B09, papel #F2EEE5, rojo Jake Mate #E63229. Tipografías: Anton (display), Fraunces (itálica editorial), Archivo (texto). Motivos: caballo de ajedrez del logo, cinta marquee con bordes de tablero (checker), texto orbital girando alrededor del logo, hero con reveal línea por línea, grano de película, parallax y tilt 3D en el logo.

## Contenido (fiel al original)
- Hero, 6 capítulos numerados: 01 La oportunidad, 02 Portafolio (Build/Grow/Automate), 03 Tarifa de referencia (14 servicios, Partner vs US Retail + fuentes Clutch/IBIZDigital), 04 Paquetes (Starter/Growth/Sales/AI Business), 05 Modelos de alianza (White Label/Co-branded/Referral), 06 Crecimiento.
- CTA: "Yafelin abre la puerta. Jake Mate hace posible la tecnología." + nota "Todo es negociable".
- Botón flotante "Guardar en PDF" (window.print) con hoja de estilos @media print completa.

## Implementado (Julio 2026)
- Propuesta HTML award-level con animaciones GSAP, scroll suave Lenis, reveals por scroll, parallax, marquee.
- Modo impresión/PDF verificado: PDF real generado por Chromium, 11 páginas A4, sin páginas en blanco, las 14 filas de precios, 4 paquetes, 3 modelos y la nota "Todo es negociable" presentes.
- Verificación visual por screenshots de todas las secciones en desktop.

## Credenciales
- No aplica: documento público sin autenticación ni backend.

## Backlog / próximos pasos posibles
- P0: ninguno bloqueante.
- P1: versión en inglés para clientes US; datos de contacto/CTA real (WhatsApp, agendar reunión) si el usuario los comparte.
- P2: variante "versión cliente final" sin columna Partner (solo retail); favicon/OG image para compartir el link con vista previa atractiva.
