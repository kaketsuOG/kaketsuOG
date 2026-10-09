<h1 align="center">Hola, soy Sebastián Espinoza 👋</h1>

<h3 align="center">Ingeniero Civil Informático · Desarrollador Full-Stack</h3>

<p align="center">
  Titulado de la Universidad Católica del Maule (Talca, Chile).<br/>
  Desarrollo puntos de venta, autoservicios, integraciones de pago y módulos para Odoo.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Ubicaci%C3%B3n-Chile-0039A6?style=flat-square" alt="Chile"/>
  <img src="https://img.shields.io/badge/Enfoque-POS%20%C2%B7%20Pagos%20%C2%B7%20Odoo-714B67?style=flat-square" alt="POS, Pagos y Odoo"/>
</p>

---

## Sobre mí

- 🎓 **Ingeniero Civil Informático**, Universidad Católica del Maule (2019 – 2025).
- 💼 Trabajo como **Desarrollador Full-Stack** en soluciones para retail y gastronomía: puntos de venta, tótems de autoservicio, agentes de pago y módulos de Odoo.
- 💳 Integro terminales y medios de pago (BCI, Getnet, Klap, Transbank, Mercado Pago) con el POS, tanto en Windows como en Android.
- 📴 Diseño sistemas **offline-first**: siguen operando sin conexión y sincronizan al recuperarla.
- 🌎 Español (nativo) · Inglés (intermedio).

## Tecnologías

**Frontend**

<p>
  <img src="https://skillicons.dev/icons?i=react,vite,tailwind,angular,ts,js,html,css" alt="Frontend"/>
</p>

**Backend y escritorio**

<p>
  <img src="https://skillicons.dev/icons?i=nodejs,express,electron,python,php" alt="Backend y escritorio"/>
</p>

**Móvil**

<p>
  <img src="https://skillicons.dev/icons?i=kotlin,androidstudio" alt="Móvil"/>
</p>

**Bases de datos**

<p>
  <img src="https://skillicons.dev/icons?i=postgres,mysql,sqlite,mongodb,supabase" alt="Bases de datos"/>
</p>

**Cloud y herramientas**

<p>
  <img src="https://skillicons.dev/icons?i=aws,vercel,git,github,postman" alt="Cloud y herramientas"/>
</p>

**También trabajo con:** Odoo 12, 16 y 18 (módulos POS, inventario y compras) · Jetpack Compose · Zustand · IndexedDB · JWT · Prisma · Sequelize · Chart.js · jsPDF · comunicación serial/USB con terminales de pago

## En qué trabajo actualmente

> La mayoría de estos repositorios son privados porque pertenecen a proyectos de clientes.

### 💳 Agentes de pago para POS integrado
Aplicaciones locales que conectan el punto de venta (Odoo POS o autoservicio) con el terminal de pago. Corren en segundo plano en la caja, exponen una API HTTP local y traducen cada venta al protocolo del terminal.

| Agente | Qué hace | Stack |
| --- | --- | --- |
| **GoBCIPagos** | Agente para BCI POS Integrado: app de bandeja con instalador, autoarranque y monitor web de logs en vivo | Node.js · Windows |
| **GoBCIPagos Android** | Port del agente BCI para tótems Android, con los mismos endpoints que la versión Windows | Kotlin · USB-serial |
| **GoGetnet** | Agente para Getnet POS Integrado, compatible con terminales atendidos y desatendidos (PAX A920 Pro e IM30) | Node.js · Serial USB / TCP |
| **GoAPIKlap** | Puente y consola de diagnóstico entre Odoo POS y el Smart POS de Klap | Electron |
| **API Mercado Pago local** | Microservicio local de Mercado Pago para POS y autoservicio | Node.js · Express · Electron |

### 🛒 Puntos de venta (PDV)
- **PDV Getit** — Punto de venta web con operación offline, almacenamiento local y emisión de comprobantes en PDF. *React · Vite · Zustand · IndexedDB · jsPDF*
- **PDV Dandi's** — Punto de venta y API intermedia offline-first para locales de yogurt helado, con impresión de tickets y arranque automático. *Node.js · Express · SQLite · Electron*

### 🖥️ Autoservicio (tótems)
- **Autoservicio Getit** — Tótem de autoatención en Android con pago integrado en el mismo equipo. *Android nativo (app de autoservicio + servicios locales de proxy y pago)*

### 📦 App de Conteo de Stock
App Android nativa para conteos de inventario con pistola lectora de códigos de barra. Descarga el catálogo desde Odoo, consolida cantidades por SKU y sincroniza los resultados; funciona offline y reenvía los conteos pendientes al recuperar conexión.
*Kotlin · Jetpack Compose · Odoo*

### 🍳 Pantallas de cocina (KDS)
Sistema de pantallas de cocina que recibe los pedidos del POS y los muestra en cocina, con impresión de comandas.
*Node.js · Express · SQLite · Electron*

### 🧩 Módulos para Odoo
Módulos que he desarrollado, en versiones de Odoo 12, 16 y 18:

| Área | Módulo | Qué hace |
| --- | --- | --- |
| **Pagos en POS** | `pos_bci_payment` | Pago con terminal BCI POS Integrado (Odoo 12 y 16) |
| | `pos_getnet_payment` | Pago con terminal Getnet POS Integrado |
| | `pos_klap` | Pago con Smart POS de Klap |
| | `pos_transbank_integration` | Pago con terminal Transbank |
| | `pos_mercadopago` | Pago con Mercado Pago (Odoo 16 y 18) |
| **Delivery** | `pos_pedidosya` | Recepción de pedidos de PedidosYa en el POS |
| | `pos_rappi` | Recepción de pedidos de Rappi en el POS |
| **Punto de venta** | `pos_credito_fiado` | Ventas a crédito (fiado) por cliente |
| | `pos_cupones` | Cupones de descuento en el POS |
| | `pos_yl_coupons` | Cupones personalizados para un cliente |
| | `verificador_precios` | Verificador de precios para consulta en tienda |
| **Reportes de caja** | `pos_informe_recaudacion` | Informe de recaudación por caja |
| | `pos_z_fondo_venta` | Informe Z por fondo de venta |
| **Inventario** | `stock_pos_scan` | Conteo de stock con escáner, conectado a la app de Conteo de Stock |
| **Compras** | `purchase_last_price_range` | Último precio de compra por rango |
| | `purchase_thermal_ticket` | Impresión de compras en ticket térmico |
| | `purchase_user_warehouse` | Bodega de compra asignada por usuario |
| **Integraciones** | `transve_praxedo` | Integración de Odoo con Praxedo |

## Otros proyectos

- **[Plataforma Web de Control de Atrasos](https://github.com/kaketsuOG/Sistema-de-control-de-asistencia-con-mensajeria-instantanea)** *(Proyecto de Título)* — Registro de atrasos en colegios con avisos por WhatsApp y reportes en PDF. *React · Node.js · PostgreSQL (Supabase) · AWS*
- **Plataforma de finanzas personales** — Ingresos, gastos, suscripciones, presupuestos y metas de ahorro con dashboards. *React · Tailwind · Express · Prisma · PostgreSQL*
- **[Tienda en línea](https://github.com/kaketsuOG/tienda)** — E-commerce con cuentas de usuario, panel con gráficos y pagos en línea. *React · Express · Supabase · Mercado Pago*
- **[Sistema de Reserva de Agua](https://github.com/kaketsuOG/Sistema_Reserva_Agua)** — Productos y reservas en línea para una distribuidora de agua. *TypeScript*
- **[Sistema de Gestión de Inventario](https://github.com/kaketsuOG/Sistema_Gestion_inventario)** — Inventario para la empresa San Pablo, en Talca. *PHP*

## Experiencia

**Desarrollador Full-Stack** — Puntos de venta, autoservicio, pagos y Odoo
*2025 – Actualidad*

**Desarrollador Full-Stack (Práctica Profesional)** — Colina Verde Ltda., Requínoa
*Enero 2025 – Marzo 2025*
Plataforma web para la gestión de maquinaria con Node.js, React y MySQL: inventario, calendario de mantenimientos con alertas, roles con JWT y dashboards de costos.

## Estadísticas

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=kaketsuOG&show_icons=true&hide_border=true&theme=tokyonight&locale=es" alt="Estadísticas de GitHub"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=kaketsuOG&layout=compact&hide_border=true&theme=tokyonight&locale=es" alt="Lenguajes más usados"/>
</p>
