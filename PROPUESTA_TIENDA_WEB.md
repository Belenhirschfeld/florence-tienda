# FLORENCE - Propuesta de Tienda Web 🛍️

**Fecha:** 3 de octubre de 2026  
**Proyecto:** Tienda online para FLORENCE Local  
**Ubicación:** Rivadavía 912, Crespo, E.R  
**Instagram:** @florencelocal (8.434 seguidores)

---

## 📋 Visión del proyecto

Crear una tienda web que:
- ✨ Refleje la identidad visual de FLORENCE (minimalista, elegante, romántico)
- 🛒 Permita a los clientes comprar online cómodamente
- 💳 Integre pasarela de pagos (Stripe/Mercado Pago)
- 👥 Gestione usuarios, órdenes y reportes
- 📱 Sea responsive y cargue rápido
- 🎯 Sea una extensión natural del local físico

---

## 🎨 Identidad visual propuesta

### Paleta de colores

| Color | Hex | Uso |
|-------|-----|-----|
| Crema principal | #FFFBF7 | Fondo principal, fondos de secciones |
| Beige cálido | #E8DDD4 | Acentos, secciones destacadas |
| Gris claro | #D9D6D0 | Separadores, bordes sutiles |
| Rosa pólvora | #D4A5A5 | CTA, acentos, botones principales (el signature color) |
| Madera natural | #A88E6B | Elementos decorativos, logos |
| Blanco | #FFFFFF | Tarjetas, superficies claras |
| Negro | #1A1A1A | Texto principal, contrastes |

### Tipografía
- **Headings:** Serif elegante (Georgia, Garamond o similar) - comunica sofisticación
- **Body:** Sans-serif limpio (Inter, Poppins) - legibilidad
- **Énfasis:** Madera natural para detalles decorativos

### Tono de voz
Cálido, accesible, elegante. Dirigiéndose a mujeres jóvenes-adultas que valoran calidad, comodidad y estilo.

---

## 🏗️ Estructura y funcionalidades (MVP)

### Frontend (Página web)

#### 1. Homepage
- Header con logo FLORENCE + navegación
- Hero section con imagen + call-to-action
- Categorías destacadas (Remeras, Pantalones, Accesorios, etc.)
- Productos destacados (últimos agregados)
- Newsletter signup
- Footer con contacto e info legal

#### 2. Catálogo de productos
- Listado con filtros (categoría, talla, color, precio)
- Búsqueda por nombre/descripción
- Ordenamiento (precio, nuevo, popular)
- Paginación
- Vista grid de productos

#### 3. Página de producto
- Imágenes del producto (multiple views)
- Descripción, materiales, care instructions
- Talla y color seleccionables
- Reviews de clientes
- Botón "Agregar al carrito"
- Productos relacionados

#### 4. Carrito de compras
- Listado de items
- Cantidad ajustable
- Eliminar productos
- Resumen de total + envío
- Proceder al checkout

#### 5. Checkout / Pago
- Información de envío
- Método de pago (Stripe/Mercado Pago)
- Confirmación de orden
- Email de confirmación

#### 6. Mi cuenta (usuarios registrados)
- Perfil / datos personales
- Historial de órdenes
- Direcciones guardadas
- Favoritos/Wishlist

#### 7. Página de contacto
- Formulario de contacto
- Info del local físico
- Mapa de ubicación
- Links a redes sociales

### Backend (Panel admin)

#### Dashboard
- Resumen de ventas (últimos 7 días, 30 días, mes)
- Órdenes recientes
- Top 5 productos

#### Gestión de productos
- Crear/editar/eliminar productos
- Upload de imágenes
- Gestionar categorías
- Inventario

#### Gestión de órdenes
- Listado de todas las órdenes
- Estados: pendiente, procesando, enviado, entregado, cancelado
- Detalles de orden
- Generar/enviar remito

#### Gestión de usuarios
- Listado de clientes
- Datos de contacto
- Historial de compras

#### Configuración
- Info de la tienda (nombre, descripción, etc.)
- Datos de contacto
- Políticas (devoluciones, envíos)
- Cupones/descuentos
- Email de notificaciones

---

## 💻 Stack tecnológico propuesto

### Frontend
- **Framework:** Next.js 14+ (React)
- **Styling:** Tailwind CSS + CSS personalizado
- **Estado:** Context API o Zustand
- **Componentes:** Shadcn/ui (customizados a paleta FLORENCE)

### Backend
- **Runtime:** Node.js
- **Framework:** Next.js API routes o Express.js
- **Base de datos:** Supabase (PostgreSQL) - gestión fácil + autenticación
- **Autenticación:** Supabase Auth

### Pagos
- **Mercado Pago API** (recomendado para Argentina)
- **Alternativa:** Stripe

### Hosting
- **Frontend:** Vercel (integración nativa con Next.js)
- **Base de datos:** Supabase
- **Costo mensual:** ~$20-40 USD

---

## 📅 Timeline y fases

### Fase 1: Setup e identidad (Semana 1-2)
- ✅ Crear proyecto Next.js
- ✅ Configurar Supabase
- ✅ Diseño del homepage y estructura base
- ✅ Sistema de componentes (siguiendo paleta FLORENCE)

**Duración:** 2 semanas  
**Salida:** Homepage funcional + sistema de design

---

### Fase 2: Catálogo de productos (Semana 3-4)
- ✅ Crear tabla de productos en BD
- ✅ Página de catálogo con filtros
- ✅ Página de detalle de producto
- ✅ Sistema de imágenes
- ✅ Búsqueda

**Duración:** 2 semanas  
**Salida:** Catálogo completo y funcional

---

### Fase 3: Carrito y checkout (Semana 5-6)
- ✅ Carrito de compras (localStorage + estado)
- ✅ Página de checkout
- ✅ Integración Mercado Pago
- ✅ Confirmación de orden
- ✅ Email de confirmación

**Duración:** 2 semanas  
**Salida:** Sistema de compra completo

---

### Fase 4: Autenticación y mi cuenta (Semana 7)
- ✅ Registro de usuarios
- ✅ Login/logout
- ✅ Perfil de usuario
- ✅ Historial de órdenes
- ✅ Wishlist (favoritos)

**Duración:** 1 semana  
**Salida:** Sistema de usuarios

---

### Fase 5: Panel admin (Semana 8-9)
- ✅ Autenticación admin
- ✅ Dashboard con métricas
- ✅ CRUD de productos
- ✅ Gestión de órdenes
- ✅ Gestión de usuarios

**Duración:** 2 semanas  
**Salida:** Panel administrativo funcional

---

### Fase 6: Testing y optimizaciones (Semana 10)
- ✅ Testing en navegadores
- ✅ Optimización de rendimiento
- ✅ SEO básico
- ✅ Seguridad
- ✅ Preparación para producción

**Duración:** 1 semana  
**Salida:** Tienda lista para lanzar

---

**Timeline total:** 10 semanas (aproximadamente 2.5 meses)

---

## 💰 Presupuesto

### Costos mensuales (después del lanzamiento)

| Item | Costo mensual |
|------|---|
| Hosting (Vercel) | $20 USD |
| Base de datos (Supabase) | $10-25 USD |
| Dominio | $12 USD/año (~$1/mes) |
| Email (SendGrid/Resend) | $0-20 USD |
| **TOTAL** | **~$40-50 USD/mes** |

### Comisiones de pago
- Mercado Pago: 2.9% + $0.30 por transacción
- Stripe: 2.9% + $0.30 por transacción

**Ejemplo:** Una venta de $100 cuesta ~$3.20 en comisiones

### Desarrollo inicial
**0% comisión** - Sin plataforma SaaS te ahorras comisiones del 1-3% por venta

**Comparación anual (asumiendo $5000/mes en ventas):**
- Shopify: $1,800 (plan) + $3,000 (6% en comisiones) = **$4,800/año**
- Solución personalizada: $240 (hosting) + $0 (sin comisiones) = **$240/año**

**Ahorro anual: $4,560 USD** 💰

---

## ✨ Diferenciales FLORENCE

### ¿Por qué esta solución?

1. **100% personalizado** - El diseño y funcionamiento es único de FLORENCE, no template genérico
2. **Sin comisiones** - Cada venta es tuya completa (después de pago)
3. **Scalable** - Crece sin límites ni costos adicionales
4. **Marca propia** - Tu sitio, tu dominio, tu experiencia
5. **Control total** - Cambios, mejoras, nuevas features cuando quieras
6. **Integrable** - Podés conectar con sistemas de inventario, email, redes sociales

### Características especiales

- 🌙 Interfaz hermosa y coherente con el local físico
- 📱 Completamente responsive (mobile-first)
- ⚡ Super rápido (carga en <2s)
- 🔒 Seguro (SSL, autenticación segura, datos protegidos)
- 📊 Analytics y reportes de ventas
- 🤖 Automatizaciones (emails, notificaciones)
- 📲 Notificaciones en tiempo real para órdenes

---

## 🚀 Próximos pasos

Si te parece bien esta propuesta:

1. **Confirmar el stack tecnológico**
   - ¿Te parece bien Next.js + Supabase + Mercado Pago?
   - ¿Algún cambio o preferencia?

2. **Recopilar información**
   - Catálogo de productos (con imágenes y precios)
   - Info de contacto y políticas
   - Datos para Mercado Pago (si aplicable)
   - Dominio (ej: florencelocal.com)

3. **Iniciar desarrollo**
   - Comenzamos con Fase 1 inmediatamente
   - Check-ins semanales con avances

4. **Cronograma**
   - Proyecto listo en 10 semanas (~junio 2026)

---

## ❓ Preguntas y dudas

**¿Puedo agregar más funcionalidades después?**  
Sí, el sistema está diseñado para crecer. Podemos agregar más features cuando quieras.

**¿Qué pasa si necesito cambios?**  
Fácil, es código nuestro. Cambiamos lo que necesites.

**¿Cuánto tiempo mantiene la tienda?**  
Es tuya. Una vez lanzada, podés operarla vos sola. Si necesitas cambios técnicos, podemos hacerlos.

**¿Seguridad y datos de clientes?**  
Supabase es enterprise-grade, cifrado end-to-end, GDPR compliant. Datos segurísimos.

---

**¿Vamos con esto? 🚀**

Esperamos tu confirmación para empezar.

*Propuesta realizada por Claude Code*  
*FLORENCE Local - Crespo, E.R*
