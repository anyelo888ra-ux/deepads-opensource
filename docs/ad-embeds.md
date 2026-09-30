# Formato de embed de anuncios

## v0.5 demo

La demo utiliza un formato visual conceptual:

@@text
deepads://embed/<ad-id>?token=<limited-token>
@@

No es un protocolo definitivo ni una credencial real.

## Reglas

- `ad-id` puede ser identificable públicamente.
- `token` debe ser limitado y revocable.
- Nunca incluir API keys, claves de base de datos o secretos administrativos.
- Los embeds reales deben generarse en el backend.
- La revocación debe ocurrir server-side.

## Renderizado

Una integración futura podrá convertir el embed en un bloque de anuncio. La etiqueta de publicidad debe seguir siendo visible.

El destino final debe pasar por las reglas de seguridad de URL antes de publicarse.
