# PROJECT STATUS — ISLE OF ORIGINS

**Última actualización:** 9 de noviembre de 2026  
**Estado general:** planificación y documentación conceptual inicial.

## 1. Resumen
El concepto, la dirección artística inicial y el alcance deseado están definidos a nivel preliminar. No se ha confirmado en esta documentación que exista una versión jugable ni que los sistemas descritos estén implementados.

## 2. Estado por área

| Área | Estado | Observación |
|---|---|---|
| Concepto e historia | Definido inicialmente | Falta desarrollar guion y misiones. |
| Dirección artística | Definida inicialmente | Ver `ART_BIBLE.md`. |
| Motor | Propuesto | Unreal Engine 5; confirmar versión y viabilidad. |
| Arquitectura técnica | Pendiente | Elegir Blueprints, C++ o enfoque híbrido. |
| Mapa y terreno | Pendiente | No hay mapa jugable verificado. |
| Control del jugador | Pendiente | Sin implementación verificada. |
| Dinosaurios e IA | Pendiente | Sin criaturas funcionales verificadas. |
| Supervivencia e inventario | Pendiente | Sin implementación verificada. |
| Multijugador | Pendiente | Objetivo de hasta 4 jugadores; no implementado. |
| Optimización | Pendiente | Requiere pruebas en el equipo objetivo. |
| Arte 3D final | Pendiente | Los conceptos visuales no equivalen a assets integrados. |

## 3. Objetivo del primer prototipo (MVP)
Construir una pequeña sección jugable que permita:
1. Iniciar una partida y controlar al personaje.
2. Explorar una zona pequeña de la isla.
3. Encontrar al menos un recurso recolectable.
4. Encontrarse con un dinosaurio funcional con comportamiento básico.
5. Recibir daño y comprobar una condición básica de supervivencia.
6. Reiniciar la prueba sin errores críticos.

El accidente aéreo puede representarse inicialmente mediante una escena breve o un punto de inicio narrativo sencillo. No construir toda la isla antes de validar el bucle jugable.

## 4. Restricciones de hardware conocidas
Equipo de referencia comunicado por el usuario:
- CPU: Intel Core i5-1135G7.
- RAM: 8 GB.
- GPU: NVIDIA GeForce GTX 1050 Max-Q, 3 GB de VRAM.

Estas especificaciones hacen necesario priorizar un prototipo pequeño y pruebas de rendimiento tempranas. Unreal Engine 5 puede resultar exigente en este equipo; evaluar una configuración reducida y, si el rendimiento no es aceptable, reconsiderar el motor o el alcance visual.

## 5. Criterios para actualizar este archivo
- Usar **Pendiente**, **En progreso**, **Implementado** o **Probado**.
- Marcar como **Probado** solo después de ejecutar la función y registrar el resultado.
- Anotar errores conocidos y limitaciones.
- Actualizar la fecha al realizar cambios relevantes.
