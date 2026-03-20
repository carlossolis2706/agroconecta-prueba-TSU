# 🌿 AgroConecta – Marketplace Local

**Prototipo funcional de interfaz de usuario para un marketplace digital orientado a productores agrícolas locales.**

> Proyecto desarrollado como parte de la estancia profesional (TSU) para la **Asociación AgroConecta Productores Unidos**, con el objetivo de conectar vendedores de productos agrícolas con compradores finales a través de una plataforma web accesible, moderna y enfocada en la experiencia del usuario.

---

## 📋 Tabla de Contenidos

- [Descripción del Proyecto](#-descripción-del-proyecto)
- [Características Principales](#-características-principales)
- [Arquitectura de Módulos](#-arquitectura-de-módulos)
- [Stack Tecnológico](#-stack-tecnológico)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Instalación y Uso](#-instalación-y-uso)
- [Roles del Sistema](#-roles-del-sistema)
- [Pantallas por Módulo](#-pantallas-por-módulo)
- [Paleta de Colores e Identidad Visual](#-paleta-de-colores-e-identidad-visual)
- [Capturas de Pantalla](#-capturas-de-pantalla)
- [Roadmap](#-roadmap)
- [Autor](#-autor)
- [Licencia](#-licencia)

---

## 🎯 Descripción del Proyecto

**AgroConecta** es un prototipo de alta fidelidad para un marketplace digital que facilita la comercialización de productos agrícolas a nivel local. El sistema abarca el flujo completo de una operación de e-commerce: desde el registro y autenticación de usuarios, pasando por la gestión de comercios y productos, catálogo con búsqueda, carrito de compras, checkout, procesamiento de pagos, seguimiento de entregas, gestión documental, reportes e indicadores, hasta un panel de administración completo.

El prototipo consta de **27 pantallas HTML interactivas** distribuidas en **9 módulos funcionales**, todas navegables entre sí a través de un Demo Navigator central que permite explorar los flujos de cada rol del sistema.

---

## ✨ Características Principales

- **Prototipo 100% navegable** — Todas las pantallas están interconectadas con navegación funcional entre módulos.
- **3 roles de usuario** — Flujos diferenciados para Comprador, Vendedor y Administrador.
- **Diseño responsive** — Adaptado a múltiples resoluciones con breakpoints para móvil, tablet y escritorio.
- **Soporte para modo oscuro** — 27 de 27 pantallas implementan dark mode vía Tailwind CSS.
- **Visualización de datos** — Dashboards con gráficos interactivos generados con Canvas API para reportes y métricas.
- **Interfaz moderna** — Diseño limpio y profesional con iconografía Material Symbols y tipografía Inter.
- **Demo Navigator** — Página central (`index.html`) con acceso rápido por rol y desglose por módulo.

---

## 🏗 Arquitectura de Módulos

```
AgroConecta
├── Módulo 1: Autenticación y Usuarios      (7 pantallas)
├── Módulo 2: Gestión de Comercio           (4 pantallas)
├── Módulo 3: Catálogo y Búsqueda           (2 pantallas)
├── Módulo 4: Pedidos y Carrito             (5 pantallas)
├── Módulo 5: Pagos y Reembolsos            (2 pantallas)
├── Módulo 6: Envíos y Entregas             (2 pantallas)
├── Módulo 7: Gestión Documental            (1 pantalla)
├── Módulo 8: Reportes e Indicadores        (1 pantalla)
└── Módulo 9: Panel Administrador           (3 pantallas)
                                     Total: 27 pantallas
```

---

## 🛠 Stack Tecnológico

| Tecnología | Uso |
|---|---|
| **HTML5** | Estructura semántica de todas las pantallas |
| **Tailwind CSS** (vía CDN) | Framework de utilidades para estilos, responsive design y dark mode |
| **JavaScript (Vanilla)** | Interactividad, animaciones, manejo de estado con `sessionStorage` |
| **Material Symbols** | Sistema de iconografía (Google Fonts) |
| **Inter** | Tipografía principal del proyecto (Google Fonts) |
| **Canvas API** | Gráficos y visualizaciones en dashboards y reportes |

> **Nota:** Este es un prototipo de interfaz (frontend estático). No incluye backend, base de datos ni lógica de servidor. Toda la interactividad se simula del lado del cliente.

---

## 📁 Estructura del Proyecto

```
agroconecta-prueba-TSU-main/
│
├── index.html                              # Demo Navigator – Página de acceso central
│
├── Modulo 1 Autenticacion y Usuarios/
│   ├── 1.1 login.html
│   ├── 1.2 Registro Selección de Rol.html
│   ├── 1.3 Formulario de Registro (Comprador).html
│   ├── 1.3.5 Formulario de Registro Ubicacion (Comprador).html
│   ├── 1.4 Formulario de Registro (Vendedor).html
│   ├── 1.5 Verificación de Correo.html
│   ├── 1.6 Mi Perfil.html
│   └── IMAGENES/
│
├── Modulo 2 Gestion de Comercio/
│   ├── 2.1 Dashboard del Vendedor.html
│   ├── 2.2 RegistroEdicion de Comercio.html
│   ├── 2.3 Lista de Productos del Vendedor.html
│   ├── 2.4 Formulario Alta/Edición de Producto.html
│   └── IMAGENES/
│
├── Modulo 3 Catalogo y Busqueda/
│   ├── 3.1 Home – Catálogo General.html
│   ├── 3.2 Detalle de Producto.html
│   └── IMAGENES/
│
├── Modulo 4 Pedidos y Carrito/
│   ├── 4.1 Carrito de Compras.html
│   ├── 4.2 Checkout / Pago.html
│   ├── 4.2.5 Procesando Pago.html
│   ├── 4.3 Historial de Pedidos (Comprador).html
│   ├── 4.4 Bandeja de Pedidos (Vendedor).html
│   └── IMAGENES/
│
├── Modulo 5 Pagos y Reembolsos/
│   ├── 5.1 Confirmación de Pago.html
│   ├── 5.2 Gestión de Reembolsos.html
│   └── IMAGENES/
│
├── Modulo 6 Envios y Entregas/
│   ├── 6.1 Seguimiento de Entrega (Comprador).html
│   ├── 6.2 Asignación de Entrega (Vendedor).html
│   └── IMAGENES/
│
├── Modulo 7 Gestion Documental/
│   ├── 7.1 Centro de Documentos.html
│   └── IMAGENES/
│
├── Modulo 8 Reportes e indicadores/
│   ├── 8.1 Reportes de Ventas.html
│   └── IMAGENES/
│
└── Modulo 9 Panel Administrador/
    ├── 9.1 Dashboard del Administrador.html
    ├── 9.2 Gestión de Usuarios y Roles.html
    ├── 9.3 Reportes Globales (Admin).html
    └── IMAGENES/
```

---

## 🚀 Instalación y Uso

Este prototipo no requiere instalación, dependencias ni compilación. Basta con abrir los archivos HTML en un navegador web moderno.

### Opción 1 – Apertura directa
```bash
# Clonar el repositorio
git clone https://github.com/tu-usuario/agroconecta-prueba-TSU.git

# Abrir el Demo Navigator en tu navegador
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

### Opción 2 – Servidor local (recomendado)
```bash
# Con Python
python -m http.server 8080

# Con Node.js
npx serve .

# Con VS Code
# Instalar la extensión "Live Server" y hacer clic en "Go Live"
```

Luego accede a `http://localhost:8080` en tu navegador.

### Requisitos
- Navegador web moderno (Chrome, Firefox, Edge, Safari)
- Conexión a internet (para cargar Tailwind CSS, fuentes e iconos desde CDN)

---

## 👥 Roles del Sistema

### 🛒 Comprador
Flujo: **Catálogo → Detalle de Producto → Carrito → Checkout → Pago → Historial de Pedidos → Seguimiento de Entrega**

Accede al marketplace para buscar productos agrícolas, realizar compras, dar seguimiento a pedidos y solicitar reembolsos.

### 🏪 Vendedor
Flujo: **Dashboard → Registro de Comercio → Gestión de Productos → Bandeja de Pedidos → Asignación de Entregas → Reportes de Ventas**

Administra su comercio, publica productos, gestiona pedidos entrantes, coordina entregas y consulta reportes de desempeño.

### ⚙️ Administrador
Flujo: **Dashboard General → Gestión de Usuarios y Roles → Reportes Globales**

Supervisa la operación completa de la plataforma, gestiona usuarios, roles y permisos, y accede a reportes e indicadores globales.

---

## 📄 Pantallas por Módulo

### Módulo 1 – Autenticación y Usuarios
| # | Pantalla | Descripción |
|---|---|---|
| 1.1 | Login | Inicio de sesión con correo y contraseña |
| 1.2 | Selección de Rol | Registro inicial con elección entre Comprador o Vendedor |
| 1.3 | Registro Comprador | Formulario de datos personales del comprador |
| 1.3.5 | Ubicación Comprador | Captura de dirección y ubicación de entrega |
| 1.4 | Registro Vendedor | Formulario de datos y documentación del vendedor |
| 1.5 | Verificación de Correo | Pantalla de confirmación de correo electrónico |
| 1.6 | Mi Perfil | Visualización y edición de datos del perfil de usuario |

### Módulo 2 – Gestión de Comercio
| # | Pantalla | Descripción |
|---|---|---|
| 2.1 | Dashboard del Vendedor | Panel principal con métricas, pedidos recientes y accesos rápidos |
| 2.2 | Registro/Edición de Comercio | Alta y configuración de la tienda del vendedor |
| 2.3 | Lista de Productos | Inventario de productos con filtros, búsqueda y acciones |
| 2.4 | Alta/Edición de Producto | Formulario para agregar o modificar productos del catálogo |

### Módulo 3 – Catálogo y Búsqueda
| # | Pantalla | Descripción |
|---|---|---|
| 3.1 | Home / Catálogo General | Página principal con barra de búsqueda, filtros y grid de productos |
| 3.2 | Detalle de Producto | Vista completa del producto con imágenes, descripción, precio y acciones |

### Módulo 4 – Pedidos y Carrito
| # | Pantalla | Descripción |
|---|---|---|
| 4.1 | Carrito de Compras | Resumen de productos seleccionados con control de cantidades |
| 4.2 | Checkout / Pago | Formulario de dirección de envío y método de pago |
| 4.2.5 | Procesando Pago | Animación de procesamiento de transacción |
| 4.3 | Historial de Pedidos | Listado de órdenes del comprador con estados y detalles |
| 4.4 | Bandeja de Pedidos (Vendedor) | Gestión de órdenes recibidas con cambios de estado |

### Módulo 5 – Pagos y Reembolsos
| # | Pantalla | Descripción |
|---|---|---|
| 5.1 | Confirmación de Pago | Resumen de transacción exitosa con detalles del pedido |
| 5.2 | Gestión de Reembolsos | Solicitud y seguimiento de devoluciones |

### Módulo 6 – Envíos y Entregas
| # | Pantalla | Descripción |
|---|---|---|
| 6.1 | Seguimiento de Entrega | Rastreo en tiempo real del estado de envío (Comprador) |
| 6.2 | Asignación de Entrega | Coordinación y asignación de entregas (Vendedor) |

### Módulo 7 – Gestión Documental
| # | Pantalla | Descripción |
|---|---|---|
| 7.1 | Centro de Documentos | Repositorio de facturas, recibos y documentos asociados |

### Módulo 8 – Reportes e Indicadores
| # | Pantalla | Descripción |
|---|---|---|
| 8.1 | Reportes de Ventas | Gráficos y tablas con métricas de ventas del vendedor |

### Módulo 9 – Panel Administrador
| # | Pantalla | Descripción |
|---|---|---|
| 9.1 | Dashboard del Administrador | Panel general con KPIs, actividad reciente y alertas |
| 9.2 | Gestión de Usuarios y Roles | CRUD de usuarios con asignación de roles y permisos |
| 9.3 | Reportes Globales | Indicadores globales de la plataforma con gráficos comparativos |

---

## 🎨 Paleta de Colores e Identidad Visual

| Rol / Contexto | Color | Hex | Uso |
|---|---|---|---|
| **Primario (Comprador)** | 🟢 Verde | `#2E7D32` | Marca principal, botones, acentos generales |
| **Vendedor** | 🟩 Verde Azulado | `#00695C` | Elementos diferenciados del rol vendedor |
| **Administrador** | 🟠 Naranja | `#E65100` | Alertas, panel de administración |
| **Fondo claro** | ⬜ Gris claro | `#FAFAFA` | Background principal en modo claro |
| **Fondo oscuro** | ⬛ Verde oscuro | `#141E15` | Background principal en modo oscuro |
| **Éxito** | 🟢 Verde brillante | `#4CAF50` | Confirmaciones, estados exitosos |
| **Info** | 🔵 Azul | `#1565C0` | Elementos informativos |

**Tipografía:** Inter (300–900) vía Google Fonts
**Iconografía:** Material Symbols Outlined (Google Fonts, variable weight 100–700)

---

## 📸 Capturas de Pantalla

Cada módulo incluye una carpeta `IMAGENES/` con capturas de referencia de las pantallas correspondientes. En total se incluyen **28 recursos gráficos** distribuidos entre los 9 módulos.

---

## 🗺 Roadmap

- [x] Prototipo de alta fidelidad (27 pantallas HTML)
- [x] Navegación completa entre módulos
- [x] Soporte para dark mode
- [x] Diseño responsive
- [x] Dashboards con visualización de datos
- [ ] Integración con backend (API REST)
- [ ] Base de datos relacional (esquema ya diseñado: 29 tablas, 1NF–5NF)
- [ ] Autenticación real (JWT / OAuth)
- [ ] Pasarela de pagos
- [ ] Geolocalización para entregas
- [ ] Notificaciones en tiempo real
- [ ] Despliegue en producción

---

## 👤 Autor

**Solis** — Estudiante de Ingeniería en Desarrollo de Software
Proyecto de Estancia Profesional (TSU)
Asociación AgroConecta Productores Unidos

---

## 📄 Licencia

Este proyecto fue desarrollado con fines académicos como parte de una estancia profesional. Todos los derechos reservados.

---

<p align="center">
  <strong>🌿 AgroConecta</strong> — Conectando el campo con tu mesa
</p>
