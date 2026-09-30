# DeepAds Open Source 📢

DeepAds es un sistema de anuncios **open source** para proyectos que quieren conseguir visibilidad sin convertir las visualizaciones en pagos directos.

## 💡 Regla de exposición

**5 visualizaciones válidas → +0,1% de exposición**

La recompensa es pequeña a propósito. Las integraciones deben documentar cómo usan ese dato.

## 📣 Ads Creator

Desde **v0.5** existe `create.html`, una interfaz pública para preparar anuncios gratis durante la etapa inicial.

Permite:
- nombre y descripción;
- URL de destino;
- imagen;
- MP4;
- generación de Ad ID;
- generación de embed demo;
- vista previa local.

También existe **`ads-demo.html`** para visualizar cómo podría aparecer un anuncio dentro de una web o aplicación.

> La v0.5 es una demo frontend. Todavía no sube archivos ni publica anuncios automáticamente.

## 🛡️ Verificación de URLs

DeepAds puede integrar **VirusTotal** desde el backend para analizar URLs antes de publicarlas. VirusTotal ofrece endpoints para enviar URLs y consultar sus reportes.

La API key de VirusTotal **nunca debe enviarse al navegador**. El frontend debe hablar con el backend de DeepAds y el backend debe hablar con VirusTotal.

Además, una detección limpia no garantiza que una URL sea segura: DeepAds debe combinar señales externas con sus propias reglas de revisión.

## 🔐 Embeds

Un embed real debe ser limitado y revocable.

**⚠️ NO COMPARTAS TU EMBED PRIVADO.**

Nunca debe contener secretos administrativos del servidor.

## 🧩 Arquitectura

```
GitHub público
  └── Web + docs + create.html + ads-demo.html
              │
              ▼ HTTPS
Vercel backend privado
  ├── campañas
  ├── anuncios
  ├── embeds
  ├── vistas
  ├── validación
  └── VirusTotal
              │
              ▼
        Base de datos
```

## 📚 Documentación

- [Conceptos](docs/concepts.md)
- [Arquitectura](docs/architecture.md)
- [Campañas](docs/campaigns.md)
- [Ads Creator](docs/ad-creator.md)
- [Embeds de anuncios](docs/ad-embeds.md)
- [Anti-abuso](docs/anti-abuse.md)
- [Seguridad](SECURITY.md)
- [Roadmap](ROADMAP.md)
- [Changelog](CHANGELOG.md)

## 🚀 Estado

**v0.5 — Ads Creator + Demo**

La interfaz pública ya puede preparar anuncios en modo demo. El siguiente trabajo es conectar el flujo con el backend privado, almacenamiento persistente, moderación y verificación server-side.

## 📜 Licencia

MIT.

🐾 Proyecto experimental de **anyelo888ra-ux**.
