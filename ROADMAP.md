# DeepAds Roadmap

## v0.1 — Base pública

- [x] Repositorio open source
- [x] Landing page
- [x] Documentación inicial
- [x] Concepto de exposición
- [x] Modelo inicial de embeds
- [ ] API real
- [ ] Base de datos
- [ ] Panel de campañas

## v0.2 — Campaigns

- [x] Crear campañas (demo frontend)
- [x] Campaign IDs (demo)
- [x] Generación de embeds (demo)
- [x] Revocación de embeds (demo local)
- [ ] Estadísticas básicas

## v0.2.1 — Owner Campaign

- [x] Campaña oficial de DeepAds
- [x] Campaign ID del owner
- [x] Embed demo del owner
- [x] No guardar embeds demo en el repositorio

## v0.3 — Validación

**Objetivo:** preparar el sistema para distinguir eventos de visualización válidos de tráfico artificial.

- [ ] Eventos de visualización
- [ ] Validación server-side
- [ ] Rate limiting
- [ ] Protección contra replay
- [ ] Reglas públicas de vistas válidas
- [ ] Identificadores de evento únicos
- [ ] Expiración de eventos
- [ ] Límites por campaña
- [ ] Registro mínimo de eventos
- [ ] Estadísticas básicas
- [ ] Demo de validación sin backend real

> La v0.3 no debe prometer que una vista es válida únicamente porque el navegador ejecutó JavaScript. La validación real debe ocurrir en el servidor.

## v0.4+ — Integraciones

- [ ] API pública
- [ ] Integración con motores de búsqueda
- [ ] Integración con tiendas de aplicaciones
- [ ] SDK/documentación para terceros
- [ ] Ads Creator (ads-create.html)
- [ ] Verificación de URLs de destino
- [ ] Watermark de DeepAds para anuncios

> El roadmap es orientativo y puede cambiar durante el desarrollo.
