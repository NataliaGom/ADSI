# Prototipo a Alto Nivel — CafItamita

## Descripción

El prototipo de alto nivel es la representación visual más cercana al producto final. Incorpora la identidad visual completa de CafItamita, una paleta de colores coherente, tipografía de marca, componentes consistentes y un flujo de usuario claro desde la autenticación hasta la confirmación y evaluación del pedido.

Este documento detalla el estado actual del proyecto en Figma, incluyendo las pantallas implementadas, decisiones de diseño y características funcionales del flujo de compra.

---

## Enlace al prototipo

[Ver prototipo de alto nivel en Figma](https://www.figma.com/design/keElFiUf8VfTBEKjNmmz0M)

*El archivo contiene 7 pantallas diseñadas en alta fidelidad con componentes reutilizables, un sistema de colores consistente y navegación entre estados de la aplicación.*

---

## Identidad visual

| Elemento | Decisión |
|---|---|
| **Color primario** | Naranja cálido `#FF7E52` |
| **Color secundario** | Gris oscuro `#3D4852` |
| **Color de fondo** | Blanco `#FFFFFF` |
| **Color neutro** | Gris claro `#9AA5B1` |
| **Color de éxito** | Verde `#80D860` |
| **Color de línea/divisor** | Gris muy claro `#E6EAEF` |
| **Placeholder de imagen** | Beige `#D9C7AC` |
| **Tipografía** | Inter (Regular, Medium, Semi Bold, Bold) |
| **Íconos** | Línea redondeada, estilo minimalista friendly |
| **Tono visual** | Cálido, accesible, moderno; optimizado para uso con una sola mano |

---

## Pantallas incluidas

| Núm. | Pantalla | Descripción | Estado |
|---|---|---|---|
| 1 | **Inicio de sesión** | Login con email y contraseña; opciones para invitado, crear cuenta y recuperar contraseña | Completa |
| 2 | **Menú principal / Catálogo** | Grid de productos con saludo personalizado, indicador "¿Lo de siempre?", barra de progreso y botones de agregar al carrito | Completa |
| 3 | **Menú con carrito** | Variante del catálogo mostrando estado dinámico del carrito (de 0 a N items) | Completa |
| 4 | **Menú general** | Grid expandido de 6 productos con barra de búsqueda posicionada en la parte inferior (diseño one-handed) | Completa |
| 5 | **Resumen de orden** | Desglose itemizado con customizaciones, selección de método de pago (Apple ID, Mastercard, PayPal), time picker para hora de recogida y botón de pago | Completa |
| 6 | **Confirma tu orden** | Resumen final compacto con: Qué se ordenó, método de pago y hora de recogida; opciones para modificar o confirmar | Completa |
| 7 | **Pantalla de éxito** | Confirmación visual con check, mensaje de agradecimiento y dato de próxima interacción | Completa |

---

## Componentes principales

### Navegación

Barra de navegación inferior con 5 tabs:
- Home (icono de hogar)
- Menú (icono de grid) — activo
- Carrito (icono de bolsa)
- Favoritos (icono de corazón)
- Configuración (icono de engrane)

Estado activo: Tab resaltado con fondo en color naranja, icono en naranja, indicador visual con barra redondeada.

### Tarjetas de producto

Componente reutilizable:
- Imagen cuadrada (placeholder beige o foto real)
- Nombre del producto
- Precio destacado en naranja
- Botón "+" en la esquina inferior derecha (naranja con icono blanco)

### Barra de búsqueda

Posicionada en la parte inferior de la pantalla (justo encima de la navegación):
- Diseño "one-handed": accesible fácilmente con el pulgar desde la base del teléfono
- Placeholder: "Buscar tu café..."
- Iconos de búsqueda (lupa) y filtros en naranja
- Fondo gris claro con sombra suave

### Botones de acción

Dos estilos:
- Primario: Fondo naranja, texto blanco, bordes redondeados (border-radius: 12px)
- Secundario: Fondo blanco, borde naranja, texto gris oscuro, bordes redondeados

### Time picker

Componente personalizado para seleccionar hora de recogida:
- Inputs numéricos para horas y minutos
- Controles arriba/abajo para ajustar valores
- Toggle AM/PM
- Visualización clara de la hora seleccionada

---

## Flujo de usuario

1. Usuario inicia sesión o accede como invitado
2. Visualiza el menú principal con saludo personalizado
3. Explora productos mediante grid o búsqueda (barra inferior one-handed)
4. Agrega items al carrito (contador se actualiza)
5. Accede al resumen de orden
6. Selecciona método de pago
7. Define hora de recogida con time picker
8. Revisa confirmación final
9. Confirma pedido
10. Ve pantalla de éxito con instrucciones de recogida

---

## Mejoras implementadas

1. Posicionamiento inferior de barra de búsqueda: Facilita el uso con una sola mano
2. Contador dinámico de carrito: Actualización visual en tiempo real
3. Time picker intuitivo: Selección de hora con controles arriba/abajo y toggle AM/PM
4. Saludo personalizado: Experiencia más humanizada y acogedora
5. Indicador de customizaciones: Desglose claro en el resumen de orden
6. Paleta de colores coherente: Naranja como acento primario en toda la app
7. Componentes reutilizables: Sistema de diseño escalable
8. Navegación clara entre pantallas: Estados y transiciones consistentes

---

## Información técnica

Herramienta utilizada: Figma

Características del archivo:
- 7 frames/pantallas en alta fidelidad
- 390x844px (tamaño estándar iPhone)
- Componentes con Auto Layout
- Iconos SVG nativos
- Sistema de colores documentado
- Fuente Inter en múltiples pesos

---

## Estado actual del proyecto

Fase: Prototipo de alto nivel — diseño visual completo

Funcionalidades implementadas (en Figma):
- Flujo completo de inicio de sesión a confirmación de pedido
- Estados visuales de componentes
- Navegación entre pantallas
- Grid de productos dinámico
- Selección de método de pago
- Time picker para hora de recogida

Pendiente de desarrollo:
- Interactividad real (prototipo Figma sin transiciones Smart Animate aún)
- Integración con backend
- Base de datos de productos
- Sistema de autenticación
- Procesamiento de pagos
- Notificaciones push
- Historial de pedidos
- Sistema de evaluación post-pedido

---

## Notas de entrega

- El archivo de Figma está organizado por pantallas, cada una a la altura x=0, 490px, 980px, etc. para fácil navegación
- Los colores principales están disponibles para copiar directamente desde cualquier elemento
- Todos los textos utilizan tipografía Inter en los pesos correspondientes
- Las imágenes de productos son placeholders beige que pueden ser reemplazadas con fotos reales
- La barra de navegación es consistente en todas las pantallas excepto la de éxito

---

## Próximos pasos recomendados

1. Convertir componentes en símbolos Figma con variantes (si no está hecho)
2. Agregar transiciones Smart Animate entre pantallas en modo prototipo
3. Realizar pruebas de usabilidad con usuarios finales
4. Iterar basado en feedback (especialmente en el time picker y barra de búsqueda)
5. Preparar handoff a desarrolladores con especificaciones CSS/medidas