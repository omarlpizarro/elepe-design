# Guía de sitio web — elepe.tech

**Formato:** sitio estático (HTML/CSS/JS), sin WordPress
**Hosting:** Donweb, hosting compartido con cPanel → subida por File Manager o FTP/SFTP
**Estilo:** corporativo y confiable
**Objetivo:** generar leads con empresas

Cómo usar esta guía: pasala completa a Claude Design en un primer mensaje (usá el prompt de la sección 6) y adjuntá ahí mismo el logo horizontal para que lo use tal cual. Los corchetes `[...]` marcan datos que todavía tenés que completar vos.

---

## 0. Identidad de marca (ya definida)

Ya tenés marca armada, así que el sitio se construye sobre eso — no se inventa nada nuevo.

- **Isotipo:** silueta de montaña + cactus enmarcada en una "C"/espiral, con una línea de puntos conectados debajo (referencia visual directa a datos). Es un buen elemento para reutilizar como gráfico de fondo sutil en el Hero, en vez de inventar ilustraciones abstractas nuevas.
- **Tagline oficial:** *"Inteligencia de datos para decisiones que generan valor"*
- **Línea secundaria (de la plancha de variantes):** *"Datos · Tecnología · Soluciones"* — sirve como copy de apoyo o para redes.
- **Las 5 líneas de servicio ya definidas en el logo:** Análisis de Datos · Cloud & Infraestructura · Gestión Documental · IA & Analítica Avanzada · Desarrollo a Medida. Estas reemplazan los placeholders genéricos que había puesto antes.

**Colores exactos** (extraídos de los archivos, no estimados):
| Uso | Nombre | Hex |
|---|---|---|
| Marca / textos oscuros / fondos dark | Azul marino | `#00152F` |
| Acento / CTAs / links / ".tech" | Celeste marca | `#0554C4` |
| Base | Blanco | `#FFFFFF` |
| Fondos alternos / bordes | Gris muy claro | `#E4E6E9` |

**Qué archivo usar dónde:**
- `Logo_principal_horizontal.png` (fondo blanco, con tagline e íconos de servicios) → header del sitio y sección hero
- `Logos_elepe.png` (versión compacta, navy sobre blanco, sin franja de íconos) → nav mobile, favicon, espacios chicos
- `Logo1_azul.png` (fondo navy, logo blanco) → footer oscuro, firma de email
- `Logo1_celeste.png` (fondo celeste, logo blanco) → banners o secciones de highlight puntuales
- `Logos_tres_blanco.png` → es una plancha de referencia de variantes, no va directo en el sitio (útil para redes sociales)

---

## 1. Estructura del sitio

Landing de una sola página con navegación por anclas (simple de construir y mantener). Más adelante, si querés hacer contenido/SEO, se puede sumar un blog aparte sin tocar esta base.

Orden de secciones:

1. **Header / Nav** — Logo + menú (Servicios · Cómo trabajo · Casos · Sobre mí · Contacto) + CTA fijo
2. **Hero** — Tagline de marca, propuesta de valor, CTA principal
3. **Servicios** — las 5 líneas ya definidas
4. **Cómo trabajo** — proceso en pasos, genera confianza B2B
5. **Casos de éxito / Resultados** — prueba social con métricas
6. **Sobre mí** — credibilidad técnica
7. **Stack / Tecnologías** — herramientas que usás
8. **Contacto** — formulario + vías directas
9. **Footer**

---

## 2. Contenido por sección

### Header
- Logo: `Logo_principal_horizontal.png` (o `Logos_elepe.png` en mobile si el horizontal no entra bien)
- CTA del nav: **"Agendar una llamada"**

### Hero
- Headline (usando la tagline oficial de marca):
  > "Inteligencia de datos para decisiones que generan valor"
- Subheadline:
  > "Desarrollo agentes de IA, infraestructura cloud y soluciones a medida para empresas que necesitan resultados, no experimentos."
- CTA primario: **"Quiero hablar sobre mi proyecto"** → ancla a Contacto
- Línea de refuerzo (trust): *"Ingeniero en sistemas · Analista de datos"*
- Elemento visual sugerido: el isotipo (montaña + cactus + línea de datos) como gráfico grande y sutil a la derecha del texto, o muy tenue de fondo

### Servicios (5 tarjetas, igual que en el logo)
1. **Análisis de Datos** — Dashboards y modelos que convierten datos en decisiones.
2. **IA & Analítica Avanzada** — Agentes de IA y modelos analíticos a medida para procesos de negocio.
3. **Desarrollo a Medida** — Software y automatizaciones adaptadas a tu operación.
4. **Cloud & Infraestructura** — Diseño, migración y administración de infraestructura en la nube.
5. **Gestión Documental** — Digitalización y organización inteligente de documentos y flujos.

*(Los agentes de IA quedan como el gancho principal del Hero, pero en la grilla de Servicios aparecen dentro de "IA & Analítica Avanzada" junto con el resto de la oferta real.)*

### Cómo trabajo (proceso en 4 pasos)
1. **Diagnóstico** — Entiendo el proceso o problema real de tu empresa.
2. **Diseño de solución** — Propuesta concreta: alcance, tecnología, tiempos.
3. **Implementación** — Desarrollo e integración de la solución.
4. **Acompañamiento** — Ajustes, soporte y mejora continua post-entrega.

### Casos de éxito (3 tarjetas, tomadas de tu experiencia real)
1. **Constructora de energía solar (Chile/España)** — Migración completa a la nube: Microsoft 365, SharePoint como gestor documental, ERP Business Central con dashboards en Power BI, y certificación ISO 27001 de seguridad de la información.
2. **Organismo público de vivienda (Jujuy)** — Sistema web de cuenta corriente en .NET con reportes en Power BI sobre SQL Server, para detectar deudores y hacer seguimiento de cobranzas por distintos canales.
3. **Empresa de materiales eléctricos (5 sucursales)** — ETL desde ERP Tango para armar dashboards de Ventas, Compras, Cobros y Flujo de Caja.

*Nota: son proyectos reales de tu trayectoria como IT Manager/analista, no como "elepe.tech" todavía — está bien presentarlos así ("En mi experiencia previa lideré...") mientras sumás los primeros casos bajo la marca. Antes de publicarlos con nombre de empresa, confirmá que no haya restricción de confidencialidad; si preferís, los dejamos genéricos por rubro como están arriba.*

### Sobre mí
- Foto profesional (no genérica de stock) — la del CV sirve de referencia de encuadre pero conviene una más actual/con mejor luz
- Bio (lista para usar):
  > "Ingeniero en Sistemas (UTN-FRT) con más de 5 años liderando infraestructura cloud y proyectos de datos como IT Manager en empresas de Argentina, Chile y España. Experiencia end-to-end: desde migrar compañías enteras a la nube hasta construir los dashboards que termina usando gerencia, compras, ventas y cobranzas."
- Certificaciones a destacar (3, las más reconocibles): Google Data Analytics Professional Certificate · AWS Cloud Practitioner Essentials · Microsoft Azure AI900 / DP900

### Stack / Tecnologías
Fila de logos (de tu CV, agrupados por tipo):
- **Cloud:** AWS · Microsoft Azure · Huawei Cloud
- **Datos & BI:** Power BI · Tableau · BigQuery · Python (Pandas, Scikit-learn, XGBoost) · R
- **Bases de datos:** SQL Server · PostgreSQL · Oracle
- **IA/ML:** Azure Machine Learning · Amazon SageMaker · Kubernetes
- **Desarrollo:** C# / .NET

### Contacto (CTA final)
- Formulario simple: Nombre, Email, Empresa, Mensaje
- Datos directos (de tu CV):
  - Email: omarlunapizarro@gmail.com
  - WhatsApp/Tel: +54 9 388 682-0764
  - LinkedIn: linkedin.com/in/olpizarro
  - GitHub: github.com/omarlpizarro
- Opcional: link a Calendly/Cal.com para agendar directamente

### Footer
- `Logo1_azul.png` + Omar Luna Pizarro · LinkedIn · GitHub · © 2026

---

## 3. Sistema de estilo visual

**Paleta de marca (ver sección 0 para el detalle):** navy `#00152F`, celeste `#0554C4`, blanco `#FFFFFF`, gris claro `#E4E6E9`.

**Tipografía:**
- Títulos: **Manrope** o **Space Grotesk** (semibold/bold) — moderna, técnica, coherente con el logo (geométrico, minimalista)
- Cuerpo de texto: **Inter** (regular/medium)

**Imágenes/ilustraciones:**
- Evitar fotos de stock genéricas
- Reutilizar el isotipo de marca (montaña + cactus + línea de datos) como elemento gráfico recurrente — por ejemplo como fondo sutil del Hero o como separador entre secciones — en vez de sumar iconografía nueva que no dialogue con el logo
- Capturas reales de dashboards (difuminadas si son de clientes) para reforzar credibilidad técnica

**Componentes UI:**
- Botones con bordes redondeados sutiles (8-10px)
- Sombras suaves, mucho espacio en blanco
- Grid limpio, máximo 2-3 columnas en desktop (ideal para 5 tarjetas de servicio: 3+2), 1 columna en mobile

---

## 4. Notas técnicas para el despliegue en Donweb

- **Subida:** por File Manager de cPanel o FTP/SFTP, a la carpeta `public_html` (o subcarpeta si el dominio está en un addon domain)
- **SSL:** activar el certificado Let's Encrypt gratuito desde cPanel para que `https://elepe.tech` funcione
- **DNS:** confirmar que elepe.tech apunte a los nameservers/IP de Donweb
- **Formulario de contacto:** al ser sitio estático, el `<form>` de HTML solo no envía nada — necesitás uno de estos:
  - Un servicio externo gratuito tipo Formspree, Web3Forms o FormSubmit (más simple, sin backend propio)
  - Un script PHP básico (cPanel soporta PHP nativamente)
  - Como fallback mínimo: botón directo a WhatsApp o `mailto:`
- **Analítica:** agregar Google Analytics o Plausible para medir de dónde vienen los leads
- **Performance:** al ser estático ya vas a tener carga muy rápida; solo cuidar el peso de imágenes (exportar los logos como WebP además del PNG)

---

## 5. Pendientes de tu lado
- [ ] Decidir si los 3 casos de éxito van con nombre de empresa o genéricos por rubro (ver nota de confidencialidad arriba)
- [ ] Foto profesional actualizada
- [ ] Confirmar tipo exacto de plan Donweb (para saber si PHP está habilitado para el formulario)

---

## 6. Prompt listo para pegar en Claude Design

```
Creá una landing page de una sola página para elepe.tech, una consultora de datos e
IA para empresas. Estilo corporativo y confiable, minimalista. Objetivo: generar
leads B2B. Voy a adjuntar el logo oficial (Logo_principal_horizontal.png) — usalo
tal cual en el header, no generes uno nuevo.

Paleta de marca (exacta, no la cambies): azul marino #00152F, celeste #0554C4,
blanco #FFFFFF, gris claro #E4E6E9 para fondos alternos.
Tipografía: títulos en Manrope o Space Grotesk (bold), cuerpo en Inter.

Tagline oficial: "Inteligencia de datos para decisiones que generan valor".

Secciones en este orden:
1. Header fijo con el logo adjunto, nav (Servicios, Cómo trabajo, Casos, Sobre mí,
   Contacto) y botón CTA "Agendar una llamada".
2. Hero: headline con la tagline oficial, subtítulo "Desarrollo agentes de IA,
   infraestructura cloud y soluciones a medida para empresas que necesitan
   resultados, no experimentos", CTA "Quiero hablar sobre mi proyecto", línea de
   trust "Ingeniero en sistemas · Analista de datos". Usar el isotipo de montaña y
   cactus del logo como elemento gráfico sutil de fondo.
3. Servicios: 5 tarjetas — Análisis de Datos, IA & Analítica Avanzada, Desarrollo a
   Medida, Cloud & Infraestructura, Gestión Documental (igual que en el logo).
4. Cómo trabajo: proceso en 4 pasos (Diagnóstico, Diseño de solución,
   Implementación, Acompañamiento).
5. Casos de éxito: 3 tarjetas — constructora de energía solar (Chile/España, migración
   a la nube + ISO 27001), organismo público de vivienda en Jujuy (sistema web +
   Power BI para cobranzas), empresa de materiales eléctricos con 5 sucursales
   (dashboards de ventas, compras y flujo de caja).
6. Sobre mí: bio "Ingeniero en Sistemas (UTN-FRT) con más de 5 años liderando
   infraestructura cloud y proyectos de datos como IT Manager en empresas de
   Argentina, Chile y España. Experiencia end-to-end: desde migrar compañías
   enteras a la nube hasta construir los dashboards que termina usando gerencia,
   compras, ventas y cobranzas", foto placeholder, y 3 certificaciones destacadas
   (Google Data Analytics, AWS Cloud Practitioner, Azure AI/Data Fundamentals).
7. Stack: fila de logos agrupados — AWS, Microsoft Azure, Huawei Cloud, Power BI,
   Tableau, BigQuery, Python, SQL Server, PostgreSQL, Oracle, Kubernetes, C#/.NET.
8. Contacto: formulario (nombre, email, empresa, mensaje) + datos directos: email
   omarlunapizarro@gmail.com, WhatsApp +54 9 388 682-0764, LinkedIn
   linkedin.com/in/olpizarro, GitHub github.com/omarlpizarro.
9. Footer con la versión del logo sobre fondo navy.

Diseño limpio, mucho whitespace, botones con bordes redondeados sutiles, sombras
suaves, totalmente responsive.
```
