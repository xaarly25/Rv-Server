
# Revival Lo Rural – Infraestructura 🌐

Este repositorio documenta la infraestructura técnica y arquitectónica del proyecto **Revival Lo Rural**, una plataforma creada para conectar trabajadores remotos y nómadas digitales con comunidades rurales.

> 🔒 Este repositorio **NO contiene el código fuente del proyecto** por razones de privacidad y seguridad. Solo incluye documentación de infraestructura.

## 🧩 Rol técnico

- Administración de servidor Linux (Debian) con Apache2
- Configuración de Apache2 + PHP + WordPress
- Seguridad avanzada:
  - Certbot + Let's Encrypt (SSL automático)
  - Firewall robusto con UFW
  - Integración Wordfence (nivel aplicación) con Fail2ban (nivel sistema)
  - Ocultación de IP real mediante proxy inverso (Cloudflare)
  - Monitoreo, logs y alertas personalizadas
- Automatización con cronjobs y scripts Bash
- Backups programados y restauración rápida

## 🔐 Seguridad aplicada

El servidor cuenta con una combinación de herramientas que mitigan ataques frecuentes:

- 🔒 HTTPS con **Certbot y Let's Encrypt**
- 🧱 Reglas estrictas con **UFW**
- 🛡️ Protección doble:
  - Wordfence → identifica ataques y bloquea a nivel WordPress
  - Fail2ban → detecta logs de Wordfence para banear IPs vía firewall 
- 🕵️‍♂️ Proxy inverso estilo **Cloudflare** para ocultar IP real
- 🚨 Alertas automáticas y bloqueos por comportamiento sospechoso

Esta combinación permite proteger tanto la infraestructura como la aplicación, evitando ataques comunes como fuerza bruta, DDoS o vulnerabilidades de plugins.

## 📐 Infraestructura general

- VPS autogestionado (alojado en Europa)
- Servicios desplegados:
  - Apache2 + PHP para sitio WordPress optimizado
  - MariaDB con copias de seguridad automatizadas
- Políticas de recuperación, actualizaciones y seguridad activa

## 📄 Documentación disponible

Revisa la carpeta `/docs` para acceder a:

- `arquitectura.png` → Diagrama general de servidores, servicios y flujos
- `resumen_tecnico.pdf` → Presentación técnica del proyecto
- `capturas/` → Imágenes ilustrativas del entorno (sin información sensible)

## 📫 Contacto

Para más detalles sobre el proyecto o posibles colaboraciones:
📧 carlos@revivallorural.com  
🔗 https://www.linkedin.com/in/carloshdezit/

