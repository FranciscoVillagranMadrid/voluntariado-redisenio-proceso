# Rediseño TO-BE – Proceso de Voluntariado

## 📘 Descripción General
Este proyecto forma parte de la actividad de **Rediseño de Procesos (AS-IS / TO-BE)**.  
El objetivo fue seleccionar un proceso existente dentro del sistema de albergues y **proponer una mejora aplicando heurísticas de rediseño** y herramientas de apoyo como **ChatGPT**.

El proceso elegido fue **Voluntariado**, que actualmente gestiona la asignación de voluntarios de manera manual, sin validaciones automáticas ni trazabilidad formal.

---

## 🔹 AS-IS: Situación Actual
**Nombre:** Proceso de Voluntariado (AS-IS)

**Descripción:**  
El voluntario se informa sobre los albergues, decide si desea participar y realiza su contribución en terreno.  
El albergue gestiona las tareas de manera independiente, sin coordinación ni confirmación automática.

**Problemas detectados:**
- Flujos separados sin comunicación directa entre actores.  
- Decisiones manuales y lentas.  
- Falta de trazabilidad y confirmaciones formales.  
- Ausencia de automatización o integración con el sistema.

---

## 🔹 TO-BE: Propuesta de Rediseño
**Nombre:** Proceso de Voluntariado (TO-BE)

**Descripción:**  
El proceso fue rediseñado para integrar al **Sistema de Ayuda** como orquestador automático, incorporando:
- Un asistente (ChatGPT) que sugiere tareas y albergues según ubicación y prioridad.  
- Validaciones tempranas de cupos y disponibilidad (*Knock-out*).  
- Ejecución en paralelo de notificaciones y registros.  
- Confirmación única al voluntario con todos los datos logísticos.  
- Subproceso de manejo de excepciones (re-asignación o lista de espera).

---

## 🧠 Heurísticas de Rediseño Aplicadas
| Heurística | Implementación |
|-------------|----------------|
| **Resequencing & Knock-Out** | Validar disponibilidad y cupos antes de continuar. |
| **Automation (ChatGPT)** | Generación automática de sugerencias y emparejamiento oferta-demanda. |
| **Parallelism** | Notificación al albergue y registro de asignación en paralelo. |
| **Contact Reduction** | Mensaje único de confirmación al voluntario. |
| **Exception Handling** | Subproceso de reasignación y lista de espera. |

---

## ⚙️ Impacto Esperado (Devil’s Quadrangle)

| Criterio | Resultado | Justificación |
|-----------|------------|----------------|
| **Tiempo** | ⬇️ | Eliminación de esperas y validaciones tempranas. |
| **Costo** | ⬇️ | Menos coordinación manual. |
| **Calidad** | ⬆️ | Trazabilidad y confirmaciones automáticas. |
| **Flexibilidad** | ≈ / ⬇️ | Leve reducción por reglas automáticas, mitigada con excepciones. |

---
## 🏁 Conclusión
El rediseño propuesto transforma un flujo manual y fragmentado en un proceso automatizado, eficiente y trazable.  
El nuevo modelo **reduce tiempos, mejora la experiencia del voluntario y garantiza transparencia en la gestión de ayuda.**
