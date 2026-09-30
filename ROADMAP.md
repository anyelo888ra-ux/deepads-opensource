# DeepAds Roadmap

## v0.1 — Base pública
- [x] Repositorio open source
- [x] Landing page
- [x] Documentación inicial
- [x] Concepto de exposición
- [x] Modelo inicial de embeds

## v0.2 — Campaigns
- [x] Crear campañas (demo frontend)
- [x] Campaign IDs
- [x] Generación de embeds demo
- [x] Revocación local

## v0.2.1 — Owner Campaign
- [x] Campaña oficial de DeepAds
- [x] Campaign ID del owner
- [x] Embed demo del owner

## v0.3 — Validación
- [ ] Eventos de visualización
- [ ] Validación server-side
- [ ] Rate limiting
- [ ] Protección contra replay
- [ ] Reglas públicas de vistas válidas
- [ ] Estadísticas básicas

## v0.4 — Backend
- [x] Backend privado separado
- [x] API de campañas
- [x] API de vistas
- [x] Validación básica
- [x] Regla 5 vistas = +0,1%
- [ ] Base de datos persistente
- [ ] Rate limiting de producción

## v0.5 — Ads Creator + Demo
- [x] `create.html`
- [x] Creación de anuncios gratis en la demo
- [x] Selector de imagen/MP4
- [x] Vista previa local
- [x] `ads-demo.html`
- [x] Formato conceptual de embed
- [x] Documentación del flujo de seguridad
- [ ] Endpoint backend para verificación de URL
- [ ] Integración server-side con VirusTotal
- [ ] Subida real de medios
- [ ] Watermark automático
- [ ] Persistencia de anuncios

## v0.6+
- [ ] Panel de moderación
- [ ] Estados pending/approved/rejected
- [ ] Estadísticas de anuncios
- [ ] Embeds reales y revocables
- [ ] API pública documentada
- [ ] Integraciones con Chronioñ
- [ ] SDK para terceros

## v1.0 — Ads Creator gratis
Objetivo: permitir crear y publicar anuncios bajo reglas claras, con seguridad server-side, sin cobrar por crear anuncios durante la etapa inicial.

- [ ] Flujo completo create → revisión → publicación
- [ ] Verificación de URL
- [ ] Moderación
- [ ] Almacenamiento persistente
- [ ] Medios de anuncio
- [ ] Embeds reales
- [ ] Estadísticas
- [ ] Anti-abuso de producción

> El roadmap es orientativo y puede cambiar durante el desarrollo.
