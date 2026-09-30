# Arquitectura

## Prototipo

La versión inicial puede funcionar como una aplicación web estática:

```
GitHub Pages
    │
    ├── Landing
    ├── Documentación
    └── Demo
```

## Arquitectura futura

Cuando DeepAds necesite operaciones dinámicas:

```
Frontend
   │
   ▼
DeepAds API
   │
   ├── Campañas
   ├── Embeds
   ├── Validación de vistas
   ├── Anti-abuso
   └── Recompensas de exposición
          │
          ▼
      Base de datos
```

## Seguridad

Los secretos de servidor deben permanecer en el backend y en variables de entorno del proveedor de despliegue.

El frontend nunca debe recibir claves administrativas.

## Integraciones

Un motor de búsqueda, una tienda de aplicaciones o un sitio web puede consumir la API y decidir cómo incorporar la exposición de DeepAds dentro de sus propias reglas.

La integración no debe convertir DeepAds en un mecanismo automático de posicionamiento absoluto.
