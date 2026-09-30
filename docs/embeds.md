# Embeds

## ¿Qué es un embed?

Un embed identifica una integración de anuncio para que un proyecto pueda mostrar una campaña.

## Regla de seguridad

Un embed debe considerarse información privada de integración.

**No lo publiques en repositorios, capturas o chats públicos.**

## Diseño recomendado

Un sistema real debería separar:

1. **Campaign ID** — identificador público de la campaña.
2. **Embed token** — identificador limitado para la integración.
3. **Server secrets** — secretos administrativos que nunca se entregan al navegador.

Los tokens deberían poder revocarse y rotarse.

## Ejemplo conceptual

```
Campaña
  └── campaign_id: público

Embed
  └── token: limitado + revocable

Backend
  └── API secret: privado
```

El formato final del embed todavía no está definido en v0.1.
