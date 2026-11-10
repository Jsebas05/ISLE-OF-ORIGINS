# TECHNICAL DOCUMENTATION — ISLE OF ORIGINS

**Estado:** decisiones técnicas pendientes de validación.

## 1. Objetivo técnico
Desarrollar primero un prototipo pequeño, estable y medible. La arquitectura debe permitir ampliar el mundo y sus sistemas sin introducir complejidad innecesaria desde el inicio.

## 2. Motor
**Propuesta inicial:** Unreal Engine 5.

Antes de iniciar producción, registrar:
- Versión exacta de Unreal Engine.
- Plantilla utilizada.
- Configuración de renderizado.
- Plugins habilitados y motivo de uso.
- Sistema de control de versiones de assets.

No actualizar la versión del motor durante una fase estable sin respaldo y prueba de compatibilidad.

## 3. Lenguaje y arquitectura
Decisión pendiente:
- **Blueprints:** útiles para prototipado rápido y lógica visual.
- **C++:** útil para sistemas centrales, rendimiento y lógica reutilizable.
- **Enfoque híbrido:** posible opción, pero debe mantenerse simple para el alcance del proyecto.

Registrar la decisión final y justificarla en este documento. Evitar crear una arquitectura compleja antes de tener un prototipo jugable.

## 4. Sistemas previstos
1. Character Controller: movimiento, cámara e interacción.
2. Health/Survival: salud y, más adelante, hambre, sed y resistencia.
3. Inventory: objetos, recursos y capacidad.
4. Resource Gathering: recolección de recursos.
5. Dinosaur AI: percepción, estados y comportamiento.
6. World/Environment: biomas, iluminación, clima y ciclo horario.
7. Mission/Progression: objetivos y descubrimientos.
8. Multiplayer: cooperativo de hasta cuatro jugadores, sujeto a evaluación técnica.

Implementar y probar cada sistema por separado antes de integrarlo.

## 5. Rendimiento y equipo objetivo
Equipo conocido: i5-1135G7, 8 GB RAM, GTX 1050 Max-Q de 3 GB.

Medidas iniciales:
- Comenzar con un mapa de prueba pequeño.
- Usar resolución y calidad de texturas moderadas.
- Configurar LODs y culling.
- Limitar luces dinámicas y efectos costosos.
- Evaluar desactivar o reducir funciones gráficas exigentes, incluyendo Lumen y Nanite cuando corresponda.
- Evitar grandes cantidades de vegetación animada y actores con IA simultáneos.
- Medir FPS, uso de RAM y VRAM en cada hito.

No prometer un rendimiento concreto sin pruebas en el equipo real.

## 6. Estructura de carpetas sugerida
La estructura definitiva dependerá del motor y de la plantilla elegida. Como punto de partida:

```text
ISLE_OF_ORIGINS/
├── Config/
├── Content/
│   ├── Blueprints/
│   ├── Characters/
│   ├── Dinosaurs/
│   ├── Environment/
│   ├── Materials/
│   ├── UI/
│   └── Audio/
├── Documentation/
├── Source/                 # Si se utiliza C++
├── README.md
├── ART_BIBLE.md
├── PROJECT_STATUS.md
├── TECHNICAL_DOCUMENTATION.md
├── DEVELOPMENT_LOG.md
├── NEXT_STEPS.md
└── AI_HANDOFF.md
```

## 7. Git y control de versiones
- Crear commits pequeños y descriptivos.
- No subir archivos temporales, cachés ni builds innecesarias.
- Configurar `.gitignore` adecuado para la versión de Unreal Engine.
- No guardar claves, tokens ni credenciales en el repositorio.
- Usar ramas para cambios grandes cuando sea necesario.
- Mantener una copia de seguridad antes de cambios estructurales.

## 8. Registro de decisiones
| Fecha | Decisión | Estado |
|---|---|---|
| Nov. 2026 | Unreal Engine 5 como motor propuesto | Pendiente de confirmar en el equipo |
| Nov. 2026 | Prototipo pequeño antes de construir la isla completa | Recomendación inicial |
| Nov. 2026 | Optimizar para hardware modesto | Requisito de diseño |
