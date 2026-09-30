# Campañas — v0.2

La v0.2 introduce el concepto de campañas y una interfaz experimental para generarlas.

## Flujo

```
Creador
  ↓
Nombre + URL
  ↓
Campaign ID
  ↓
Embed token
  ↓
Integración futura
```

## Demo de GitHub Pages

La implementación actual es **solo frontend** y usa `localStorage`.

Por eso:

- no crea campañas en un servidor;
- no registra visualizaciones reales;
- no ofrece seguridad de backend;
- la revocación solo cambia el estado local de la demo.

## Implementación futura

El backend deberá:

1. generar Campaign IDs;
2. generar tokens limitados;
3. almacenar campañas;
4. permitir revocación;
5. validar permisos;
6. registrar eventos de forma segura.

Los secretos administrativos nunca deben enviarse al navegador.

## Token de embed

El token mostrado por la demo es deliberadamente un token de ejemplo. Una implementación real debe usar tokens con permisos mínimos, expiración o revocación y protección contra reutilización indebida.
