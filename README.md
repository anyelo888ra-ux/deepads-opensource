# DeepAds Open Source 📢

DeepAds es un sistema de anuncios **open source** pensado para proyectos que quieren conseguir visibilidad sin convertir las visualizaciones en pagos directos.

## 💡 ¿Cómo funciona?

Una campaña puede obtener una pequeña mejora de exposición cuando consigue visualizaciones válidas:

**5 visualizaciones válidas → +0,1% de exposición**

La recompensa es pequeña a propósito: DeepAds busca evitar que unas pocas campañas dominen las recomendaciones.

### 🚫 No es un sistema de pago por ver anuncios

DeepAds no promete dinero por visualizar anuncios. La recompensa consiste en una pequeña mejora de descubrimiento dentro de los servicios que integren DeepAds, por ejemplo:

- 🔎 motores de búsqueda
- 📱 tiendas de aplicaciones
- 🌐 sitios web y proyectos de la comunidad

La integración decide cómo se aplica exactamente esa exposición.

## 🔐 Embeds y seguridad

Cuando un creador genere un anuncio, DeepAds podrá entregar un **embed privado** para instalarlo en su proyecto.

**⚠️ ADVERTENCIA: NO COMPARTAS TU EMBED PRIVADO.**

El embed puede contener identificadores o credenciales de integración que permitan asociar las visualizaciones con tu campaña y sus beneficios. Trátalo como una clave privada y no lo publiques en repositorios, capturas de pantalla ni chats públicos.

> Un embed privado nunca debería contener secretos de servidor de alto privilegio. Las implementaciones deben usar identificadores limitados y revocables.

## 🛡️ Protección contra abuso

El proyecto está diseñado con seguridad y transparencia como objetivos:

- detectar o limitar vistas artificiales;
- evitar que simples recargas generen recompensas ilimitadas;
- separar anuncios patrocinados de resultados normales;
- documentar cómo se calcula la exposición;
- minimizar los datos necesarios para validar una vista;
- mantener el código público y auditable.

Ningún sistema puede garantizar seguridad absoluta. DeepAds busca ser **security-first y auditable**.

## 🧩 Open source

DeepAds está pensado para que otras personas puedan:

- crear sus propias implementaciones;
- adaptar el sistema a sus sitios o aplicaciones;
- auditar el código;
- proponer mejoras;
- construir integraciones nuevas.

## 📚 Documentación

La documentación del proyecto está en [docs/](docs/README.md).

- [Conceptos](docs/concepts.md)
- [Arquitectura](docs/architecture.md)
- [Embeds](docs/embeds.md)
- [Anti-abuso](docs/anti-abuse.md)
- [Integraciones](docs/integrations.md)
- [Política de seguridad](SECURITY.md)
- [Roadmap](ROADMAP.md)
- [Changelog](CHANGELOG.md)

## 🚀 Estado

**v0.1 — prototipo inicial**

La primera versión se centrará en la web pública, la creación de campañas y el sistema básico de embeds.

## 📜 Licencia

DeepAds Open Source está publicado bajo la licencia MIT.

---

🐾 Proyecto experimental de **anyelo888ra-ux**.
