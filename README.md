# Registro de uso de herramientas de IA generativa

**Trabajo Fin de Máster:** Predicción de viento con Machine Learning y Deep Learning: despliegue MLOps para la activación de seguridad en paneles solares
**Autor:** Álvaro Chuecos Díaz
**Máster:** Big Data y Ciencia de Datos (VIU), curso 2025-2026
**Código del trabajo:** https://github.com/alvarochuecosd-spec/tfm-prediccion-viento/tree/v1.0

Este repositorio complementa el Anexo B de la memoria. Las herramientas de IA se han utilizado de forma continuada durante varios meses, por lo que no se conserva un registro completo de todas las interacciones. En su lugar se recogen las conversaciones principales que se han podido recuperar del historial y una tabla resumen por tipo de tarea.

Los *prompts* de la tabla son **literales**, copiados del historial sin corregir (incluidas las erratas). Donde no ha sido posible recuperar un *prompt* real, la celda queda marcada como pendiente en lugar de reconstruirse.

## Tabla resumen

| Herramienta | Periodo | Tipo de tarea | *Prompt* representativo (literal) | Conversación | Qué hizo el autor con el resultado |
|---|---|---|---|---|---|
| Claude | Abril 2026 | Orientación inicial sobre MLOps y posible enfoque del TFM | "como harías un TFM sobre etso?" · "lo veo demasiado tocho este TFM, no se como lo ves, pero ten en cuenta que soy un alumno y hay muchos conceptos qu eno tengo" | [Conversación 1](https://claude.ai/share/7cf7a8f7-8cb1-4a43-b2c8-b23bebdf433c) | Consideró la propuesta inicial demasiado amplia y pidió reducirla a un alcance realista para un TFM. |
| Claude | Junio 2026 | Fuentes de datos meteorológicos y definición del alcance | "quiero encararlo para el TFM, pero que sea aplicable en cualquier punto de España o del mundo para poder comerzializarlo" · "eso es demasiado para el alcance de mi TFM, quiero empezar por conseguir mejorar las predicciones en un lugra en concreto, para quizás ampliarlo luego" | [Conversación 2](https://claude.ai/share/5a3d991c-90bb-45bd-a3ba-9394a5e1bc98) | Decidió limitar el trabajo a un único emplazamiento y dejar la generalización como trabajo futuro. |
| GitHub Copilot | Septiembre 2026 | Formato de figuras en los notebooks (gráfica ACF/PACF del notebook `2_EDA`) | "como puedo aumentar el tamaño de las letras de esta gráfica?" · "por que correlación no sale a la msima ditancia del eje en el primer eje y en el segundo?" | [chat_copilot.json](chat_copilot.json) | Ajustó el formato de la gráfica ACF/PACF (Figura 4.1 de la memoria) a partir de las sugerencias. |
| Claude | Septiembre 2026 | Revisión de la redacción capítulo a capítulo | "ve pasásandome capitulo a capitulo lo que has cambiado y por qué:" | [Conversación 3](https://claude.ai/share/738bc705-b29d-47e5-8bd5-12970e8564f4) | Revisó los cambios propuestos, volvió a ejecutar los notebooks y contrastó cada cifra con sus salidas. Corrigió afirmaciones de la IA que no coincidían con sus datos. |
| Claude | Septiembre 2026 | Evaluación respecto al umbral (objetivo 3) | "que es lo del objetivo 3?" | [Conversación 3](https://claude.ai/share/738bc705-b29d-47e5-8bd5-12970e8564f4) | Ejecutó en el notebook 6 la celda de *recall*, precisión y F2 propuesta, aportó las salidas y las incorporó a la Sección 5.6. |
| Claude | Septiembre 2026 | Actualización de figuras y del texto asociado | "esta imagen ha cambiado" | [Conversación 3](https://claude.ai/share/738bc705-b29d-47e5-8bd5-12970e8564f4) | Regeneró la captura del panel con el modelo desplegado y actualizó las cifras citadas en el texto. |
| Claude | Septiembre 2026 | Detección de incoherencias y erratas en la versión final | "así es cómo está mi TFM, ves alguna incongruencia o errata a lo largo del texto? crees que el tono empleado es correcto?" | [Conversación 4](https://claude.ai/share/f8a9a5d2-8362-4a0b-8eac-59f8213db50e) | Rebatió la observación de que DVC y Evidently no estaban desplegados y comprobó en el código qué métodos de `statsmodels` se usaban antes de aceptar la redacción. |
| Claude | Septiembre 2026 | Redacción de la declaración de uso de IA | "para el uso de ia tengo esta infromación:" | [Conversación 3](https://claude.ai/share/738bc705-b29d-47e5-8bd5-12970e8564f4) | Completó con sus propios datos las partes que la IA no podía conocer (otras herramientas, versiones, fechas). |
| Claude | Octubre 2026 | Preparación de este registro a partir del historial | Conversación en la que se recuperaron los *prompts* de esta tabla | [Conversación 5](https://claude.ai/share/68d53135-8db1-4a6a-be50-17df1330da8f) | Revisó la tabla y completó los huecos marcados como pendientes. |

## Conversaciones exportadas

1. [Orientación inicial sobre MLOps y enfoque del TFM](https://claude.ai/share/7cf7a8f7-8cb1-4a43-b2c8-b23bebdf433c) (abril 2026)
2. [Fuentes de datos y definición del alcance](https://claude.ai/share/5a3d991c-90bb-45bd-a3ba-9394a5e1bc98) (junio 2026)
3. [Revisión completa de la memoria, objetivo 3 y Anexo B](https://claude.ai/share/738bc705-b29d-47e5-8bd5-12970e8564f4) (septiembre 2026)
4. [Revisión de incoherencias y tono de la versión final](https://claude.ai/share/f8a9a5d2-8362-4a0b-8eac-59f8213db50e) (septiembre 2026)
5. [Preparación de este registro](https://claude.ai/share/68d53135-8db1-4a6a-be50-17df1330da8f) (octubre 2026)
6. [chat_copilot.json](chat_copilot.json) Sesión de GitHub Copilot Chat en VS Code, modo agente con selección automática de modelo (17 de septiembre de 2026)

## Limitaciones del registro

El registro no es exhaustivo. Recoge las conversaciones que se han podido recuperar y exportar al final del trabajo, organizadas por tipo de tarea. Las consultas breves y puntuales (dudas de sintaxis, errores de instalación, formato de LaTeX) no se han incluido una a una.
