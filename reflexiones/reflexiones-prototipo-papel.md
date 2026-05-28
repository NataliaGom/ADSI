# Reflexión — Hallazgos del Prototipo a Papel

## Resumen de las pruebas

Se realizaron **3 pruebas de usabilidad** con el prototipo a papel de CafItamita. Los participantes representaron los tres perfiles de usuario identificados en las personas (estudiante, docente y estudiante trabajador). Cada sesión incluyó 3 tareas específicas y una entrevista breve al finalizar.

---

## Hallazgos por categoría

### Lo que funcionó bien

- **El flujo lineal fue intuitivo:** Los 3 participantes siguieron el flujo de pantallas sin perderse. La secuencia Menú → Carrito → Pago → Hora → Confirmación fue comprendida de manera natural.
- **La pantalla de confirmación:** Los usuarios valoraron ver un resumen completo antes de confirmar, esto les generó confianza en el pedido.
- **Pantallas de Menú y "¿Algo extra?":** Fueron descritas como muy claras y fáciles de entender por los participantes.
- **Mecanismo de selección de tarjeta:** El proceso de pago fue considerado sencillo e intuitivo.

---

### Problemas identificados

| # | Problema | Severidad | Frecuencia | Pantalla |
|---|---|---|---|---|
| 1 | No era posible seleccionar más de un producto en una sola sesión; después de "¿Algo extra?" se iba directamente al resumen | 3 | 3/3 usuarios | Flujo completo |
| 2 | El esquema de colores original generaba saturación visual; los participantes asociaban más los colores café y naranja con una app de café | 2 | 2/3 usuarios | Todas las pantallas |
| 3 | No había suficientes opciones de productos; no se sentía realista | 3 | 1/3 usuarios | Menú |


> **Severidad:** 1 = Cosmético, 2 = Problema de usabilidad, 3 = Bloqueador

---

### Insights cualitativos

-Los usuarios expresaron que la saturación de los colores fue lo que más les dificultaba concentrarse al incio en qué debían hacer.

---

## Cambios a realizar para el prototipo de medio nivel

A partir de los hallazgos anteriores, se realizarán las siguientes mejoras:

1. **Permitir seleccionar múltiples productos:** Después de la pantalla "¿Algo extra?", regresar al usuario a la pantalla de menú en lugar de ir directamente al resumen. Actualizar el botón "Ir al carrito" para que muestre dinámicamente el número de productos actuales en el carrito.

2. **Revisar el esquema de colores:** Cambiar de la paleta original a un esquema de **naranja y blanco únicamente**, eliminando la saturación de colores y mejorando la asociación con una app de café.

3. **Añadir más productos:** Incluir más tipos de cafés y algún snack.

---

## Conclusión

El prototipo a papel validó que la estructura y el flujo general de CafItamita son comprensibles para los tres tipos de usuario. Los problemas encontrados son principalmente de diseño visual, retroalimentación y restricciones del flujo, no de arquitectura de información. La sensación general fue positiva respecto a la intuitividad de las pantallas clave. Esto indica que la propuesta conceptual es sólida y puede iterarse con confianza en el siguiente nivel de fidelidad.