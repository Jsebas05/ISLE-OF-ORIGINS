# AI HANDOFF — ISLE OF ORIGINS

Este documento permite que otra IA o desarrollador continúe el proyecto sin asumir que las funciones previstas ya están implementadas.

## 1. Rol esperado
Actúa como desarrollador senior de videojuegos y especialista en Unreal Engine. Trabaja de forma incremental, explica las decisiones técnicas y entrega instrucciones precisas para un desarrollador que está aprendiendo.

## 2. Contexto del juego
ISLE OF ORIGINS es un videojuego de supervivencia, exploración y aventura. Tras un accidente aéreo, el jugador llega a una isla donde una organización realizó experimentos genéticos con dinosaurios. El objetivo narrativo es explorar, sobrevivir y descubrir la verdad detrás de las instalaciones.

Objetivo de modos: individual y cooperativo de hasta cuatro jugadores. El multijugador es una meta, no una función confirmada.

## 3. Dirección artística
- Estilo semi-realista y cinematográfico.
- Dinosaurios de inspiración naturalista con presencia visual memorable.
- Isla hermosa y exuberante de día, inquietante y peligrosa de noche.
- Naturaleza invadiendo instalaciones científicas abandonadas.
- Consultar `ART_BIBLE.md` antes de proponer nuevos diseños.

## 4. Estado técnico conocido
- Motor propuesto: Unreal Engine 5; versión exacta pendiente.
- Arquitectura: pendiente de decisión entre Blueprints, C++ o enfoque híbrido.
- No hay sistemas jugables confirmados en esta documentación.
- No asumir que existen modelos 3D, animaciones, mapas ni código funcional.
- Consultar `PROJECT_STATUS.md` y `DEVELOPMENT_LOG.md` para el estado actualizado.

## 5. Hardware objetivo
- Intel Core i5-1135G7.
- 8 GB RAM.
- NVIDIA GeForce GTX 1050 Max-Q con 3 GB VRAM.

Diseñar y probar con presupuestos modestos de memoria y renderizado. Recomendar cambios gráficos basados en mediciones, no en suposiciones.

## 6. Forma de trabajar
1. Revisar primero todos los documentos del repositorio.
2. Inspeccionar el proyecto existente antes de modificarlo.
3. No reiniciar ni reemplazar trabajo previo sin una razón técnica y autorización.
4. Identificar una tarea pequeña y verificable.
5. Explicar qué archivos se crearán o modificarán.
6. Implementar la tarea.
7. Ejecutar pruebas o indicar claramente qué no pudo probarse.
8. Registrar resultados, errores y pasos siguientes.
9. Actualizar la documentación afectada.
10. Proponer un commit descriptivo.

No declarar una funcionalidad como terminada si no fue probada.

## 7. Primera tarea recomendada
Comprobar el estado real del repositorio y del proyecto del motor. Después, recomendar la configuración mínima viable para crear un mapa de prueba y un personaje controlable en el hardware disponible.

No empezar creando la isla completa, todos los dinosaurios ni el multijugador. Primero validar el prototipo.

## 8. Prompt para iniciar una sesión de continuación
Lee `README.md`, `ART_BIBLE.md`, `PROJECT_STATUS.md`, `TECHNICAL_DOCUMENTATION.md`, `DEVELOPMENT_LOG.md` y `NEXT_STEPS.md`. Inspecciona el contenido real del repositorio y determina qué existe y qué funciona. No supongas que las funciones planeadas están implementadas. Resume el estado verificado y continúa con la tarea prioritaria más pequeña, explicando los cambios y las pruebas necesarias.
