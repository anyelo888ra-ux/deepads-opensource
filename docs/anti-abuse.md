# Vistas válidas y anti-abuso

DeepAds necesita distinguir entre visualizaciones reales y tráfico artificial.

## Amenazas consideradas

- recargas repetidas;
- automatización;
- duplicación o replay de eventos;
- tráfico generado por scripts;
- intentos de inflar una campaña.

## Ideas para una implementación futura

- rate limiting;
- eventos con identificadores únicos;
- timestamps y expiración;
- validación en servidor;
- límites por campaña;
- detección de patrones anómalos;
- auditoría de cambios.

## Privacidad

La validación debería recopilar únicamente los datos necesarios para proteger el sistema.

No se debe diseñar el sistema alrededor de la recopilación innecesaria de información personal.

## Recompensas

La regla propuesta es:

**5 vistas válidas → +0,1% de exposición**

La implementación debería establecer límites y reglas claras para evitar que el beneficio crezca sin control.
