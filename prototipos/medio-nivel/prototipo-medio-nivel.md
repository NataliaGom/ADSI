# Prototipo a Medio Nivel — CafItamita

## Descripción

El prototipo de medio nivel incorpora las mejoras estructurales e interactivas identificadas en las pruebas del prototipo a papel. En esta versión digital interactiva se ha implementado un esquema de color limpio que evita la saturación visual, se expandió el catálogo con más opciones de bebidas para aportar realismo y se habilitó un flujo interactivo que permite la selección y acumulación de múltiples productos en el carrito.

---

## Enlace al prototipo

[Ver prototipo de medio nivel en Moqups](https://app.moqups.com/ZmagLNrVttPI8GlAS684ResvdvK48jwu/view/page/a69490639)

*El enlace te lleva al prototipo interactivo navegable donde puedes explorar el flujo completo de compra.*

---

## Pantallas incluidas

| Num. | Pantalla | Descripción |
| --- | --- | --- |
| 1 | **Iniciar sesión** | Campos de Correo y Contraseña, acceso como invitado, enlace de recuperación de contraseña y opción de crear cuenta. |
| 2 | **Registrarse** | Formulario de alta para nuevos usuarios con campos de email, contraseña y aceptación de Términos y Condiciones. |
| 3 | **Menú principal (¿Lo de siempre?)** | Catálogo de bebidas con saludo personalizado, indicador de sección frecuente y múltiples opciones de café con precios visibles. |
| 4 | **Selección de producto / Carrito** | Interfaz interactiva que permite agregar ítems con botón "Ir al carrito" dinámico y contador de artículos actualizados en tiempo real. |
| 5 | **Resumen de tu orden** | Desglose unificado del carrito con listado de productos, precios, método de pago y selector de hora de recogida. |
| 6 | **Confirma tu orden** | Pantalla de validación final con resumen completo (productos, pago, horario) antes de confirmar la compra. |
| 7 | **Éxito del pedido** | Confirmación visual con fondo verde, ícono de verificación y mensaje de agradecimiento que cierra el flujo de compra. |

---

## Decisiones de diseño (medio nivel)

- **Esquema de colores unificado:** Paleta de naranja y blanco que facilita la concentración del usuario y refuerza la identidad de marca de café.

- **Ampliación del catálogo:** Múltiples variedades de bebidas (Capuccino mediano/grande, Latte, Frappé) con precios explícitos para simular un entorno comercial realista.

- **Selección e interacción dinámicas:** Botón "Ir al carrito" que cambia visualmente (color sólido) e incrementa un contador numérico cuando el usuario agrega productos.

- **Simplificación del flujo de compra:** Integración del carrito, selección de método de pago y ajuste de horario en un embudo ágil que evita pantallas innecesarias.

- **Accesibilidad en móvil:** Elementos interactivos primarios (botones de acción) dimensionados para garantizar zonas de toque cómodas en dispositivos móviles.

- **Jerarquía visual clara:** Uso estratégico de tipografía, espaciado y color para guiar la atención del usuario hacia acciones clave.

---

## Flujo de usuario

```
Iniciar sesión
  |
  +-- Registrarse (Crear una cuenta)
  |
  +-- Menú principal (¿Lo de siempre?)
        |
        +-- Selección de productos
              |
              +-- Botón "Ir al carrito" + Contador dinámico
                    |
                    +-- Resumen de tu orden
                          (Carrito + Método de pago + Hora de recogida)
                          |
                          +-- Confirma tu orden
                                (Revisión final de todos los datos)
                                |
                                +-- Éxito del pedido
                                      (Confirmación con ícono de check)
```

---

## Componentes principales

- **Campos de entrada:** Email, contraseña, búsqueda
- **Botones de acción:** Iniciar sesión, crear cuenta, agregar al carrito, pagar, confirmar
- **Selectores:** Método de pago (radio buttons), hora de recogida (time picker)
- **Indicadores:** Contador de carrito, barra de progreso en flujos multi-paso
- **Tarjetas:** Resumen de productos con foto, nombre y precio

---

## Herramienta utilizada

Moqups — Diseño de wireframes digitales interactivos con paleta de color aplicada, componentes reutilizables y prototipo navegable para pruebas de usuario.

---

## Estado actual

Fase: Prototipo de medio nivel — estructura interactiva con identidad visual básica

Este prototipo valida:
- Flujo de compra completo desde login hasta confirmación
- Interacción dinámica del carrito
- Selección de opciones de pago
- Selección de horario de recogida
- Estados visuales de componentes

Próximas iteraciones:
- Expansión a prototipo de alto nivel en Figma con componentes avanzados
- Pruebas de usabilidad con usuarios finales
- Refinamiento basado en feedback