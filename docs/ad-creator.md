# Ads Creator — v0.5

La v0.5 añade una experiencia pública para **crear anuncios gratis** y una página `ads-demo.html` para visualizar cómo podrían aparecer.

## Flujo

@@text
Creador
  ↓
create.html
  ↓
Nombre + URL + imagen/MP4
  ↓
Validación de formato
  ↓
Verificación de URL en backend
  ↓
Revisión/estado de seguridad
  ↓
Ad ID + embed limitado
  ↓
Integración
@@

## VirusTotal

VirusTotal se propone como **señal de reputación**, no como garantía absoluta.

El backend debe:

1. recibir la URL;
2. enviarla al endpoint de análisis de URL de VirusTotal;
3. consultar el análisis/reporte;
4. normalizar resultados;
5. aplicar las reglas propias de DeepAds;
6. devolver al frontend un estado de revisión.

La API de VirusTotal usa una API key mediante el header `x-apikey`. La clave **no debe aparecer en `create.html` ni en JavaScript público**.

## Privacidad y uso

Las URLs enviadas a la API pública pueden incorporarse al dataset de VirusTotal. No se deben enviar secretos, PII ni URLs confidenciales. La API pública también tiene límites de uso y condiciones específicas.

## Medios

v0.5 permite seleccionar imágenes y MP4. La demo solamente muestra una vista previa local. El almacenamiento real requiere backend/storage.

## Watermark

Durante la etapa inicial, los anuncios publicados pueden llevar `Powered by DeepAds`.

## Estado

v0.5 es una fase de UX + contrato de integración. Todavía no significa que un anuncio quede publicado automáticamente ni que una URL esté garantizada como segura.

## Embed

El embed real debe ser limitado, revocable y rotatable, sin secretos administrativos.
