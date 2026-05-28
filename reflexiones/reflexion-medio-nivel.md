# Reflexión — Hallazgos del Prototipo de Medio Nivel

## Contexto

Tras aplicar las iteraciones iniciales, se realizó una **prueba de navegación cuantitativa y visual** utilizando un prototipo digital interactivo en Figma con una muestra de 5 participantes. La tarea crítica evaluada fue: *"Inicia sesión, selecciona un capuccino mediano y paga por él con tu Apple ID"*. Esto permitió medir la efectividad del flujo, identificar puntos de fuga en el embudo de conversión y analizar el comportamiento visual mediante mapas de calor.

---

## ¿Qué mejoró respecto al prototipo anterior?

| Elemento Evaluado | Comportamiento en la Prueba | ¿Resuelto? |
| --- | --- | --- |
| Acceso al sistema (Login) | Flujo directo, 100% de éxito en el paso inicial | Sí |
| Selección de producto base | Clics concentrados directamente en el ítem deseado | Sí |
| Cierre del flujo de pago | Pasos finales (5 y 6) con 100% de efectividad y rapidez | Sí |
| Interacción con Apple ID | Procesamiento del pago intuitivo y sin desviaciones | Sí |

---

## Nuevos hallazgos

### Lo que funcionó bien

* **La eficiencia de las pantallas extremas:** El inicio de sesión (Paso 1) y la pantalla de éxito final (Paso 6) funcionaron de manera impecable, registrando un 100% de clics correctos y tiempos de respuesta muy bajos (entre 2 y 5 segundos).
* **Velocidad de ejecución ideal:** Aquellos usuarios que lograron completar el flujo sin desviarse lo hicieron en un tiempo sobresaliente (promedio de 20 segundos totales), lo que demuestra que la arquitectura de la ruta crítica es veloz.
* **Percepción subjetiva de facilidad:** De manera unánime (100%), los usuarios declararon no haber sentido confusión con ninguna pantalla, lo que indica que la interfaz se siente familiar y amigable a primera vista.

---

### Nuevos problemas identificados

| # | Problema | Severidad | Frecuencia | Pantalla |
| --- | --- | --- | --- | --- |
| 1 | **Caída crítica en el embudo (Selección de Tamaño):** El éxito cae al 50% en los pasos 3 y 4 debido a la confusión entre variantes del producto en la misma cuadrícula. | 3 | 3/5 usuarios | Principal / Menú |
| 2 | **Tipografía / Tamaño de letra reducido:** Los textos de las variantes son demasiado pequeños, lo que propició que se eligiera el tamaño equivocado del café por error. | 2 | 1/5 usuarios | Principal / Menú |
| 3 | **Fricción por micro-interacciones en el tiempo:** El mapa de calor muestra una saturación excesiva de clics en las flechas y el selector manual AM/PM para la hora de recogida. | 2 | 5/5 usuarios | Resumen de orden |
| 4 | **Riesgo por proximidad de acciones:** El botón "Modificar mi pedido" tiene un peso visual alto y está demasiado cerca de "Confirmar", amenazando con desvíos accidentales. | 2 | Observado en mapa de calor | Confirmación de orden |
| 5 | **La paradoja del error invisible:** Los usuarios cometen errores de selección (variante errónea) pero su percepción es de "cero confusión", ocultando el fallo operativo. | 2 | 5/5 usuarios | Global |

> **Severidad:** 1 = Cosmético, 2 = Problema de usabilidad, 3 = Bloqueador

---

### Insights cualitativos

> * *"Ninguna pantalla me confundió"* — El 100% de los participantes reportó comodidad absoluta; sin embargo, la tasa de éxito real del flujo ideal fue del 20%. Esto confirma que los errores ocurren por falta de claridad visual (UI) y no por mala navegación (UX).
> * *"Pequeño"* — Retroalimentación directa sobre elementos de la interfaz, validando que el tamaño de la letra en la selección de productos está afectando la toma de decisiones correctas.
> * *Preferencia de intervalos:* El 60% de los usuarios prefiere ajustar su hora de recogida en bloques de **5 minutos** y el 40% en bloques de **10 minutos**. Ninguno desea el control por minuto individual.
> 
> 

---

## Cambios a realizar para el prototipo de alto nivel

1. **Rediseñar la arquitectura de selección de tamaño:** Eliminar las variantes duplicadas (`Capuccino M` y `Capuccino L`) de la pantalla principal. Dejar una sola tarjeta por producto y mover la selección de tamaño y complementos a una **pantalla secundaria o ventana modal dedicada** para evitar errores de selección en el grid rápido.
2. **Optimizar la escala tipográfica:** Aumentar significativamente el tamaño de la letra y los contrastes en los nombres de los productos, precios y variables para mitigar los problemas de legibilidad reportados.
3. **Simplificar el selector de horario:** Reemplazar el sistema manual de flechas finas y botones AM/PM por un selector rápido basado en los bloques preferidos por el usuario (botones dedicados de +5 min / +10 min) o slots automáticos.
4. **Modificar la jerarquía visual en la confirmación:** Darle un ancho completo y mayor prominencia al botón de "Confirmar", reduciendo el peso visual del botón "Modificar mi pedido" a un enlace de texto o un botón secundario más alejado para evitar clics accidentales.

---

## Conclusión

La prueba cuantitativa reveló que aunque la estructura y el concepto general de **CafItamita** resultan sumamente atractivos y cómodos para el usuario, el diseño de interfaz actual genera errores silenciosos. La drástica caída en los pasos intermedios demuestra que la selección de producto y tamaño debe separarse. El prototipo de alto nivel se concentrará en limpiar el menú principal, implementar la selección mediante modales y optimizar el selector de tiempo para transformar esa buena percepción subjetiva en una tasa de éxito real mucho más alta.
