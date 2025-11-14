# Rediseño TO-BE – Proceso de Voluntariado
Martin Araya Riquelme - 21.624.104-5  
Francisco Villagrán Madrid - 21.483.516-9  
Gladys Carvacho - 21.205.052-0  

## 1. Descripción General
Este proyecto corresponde al análisis y rediseño del proceso de Voluntariado del sistema de albergues.  
El objetivo fue comprender el funcionamiento actual (AS-IS) y proponer un diseño mejorado (TO-BE) utilizando buenas prácticas de rediseño y una correcta separación de responsabilidades entre los actores.

El proceso elegido fue el de Voluntariado, debido a que actualmente funciona de manera manual, con poca claridad en las responsabilidades y sin validaciones formales de disponibilidad.

---

## 2. AS-IS: Situación Actual

### Descripción general del proceso actual
El voluntario ingresa al portal, revisa información básica y decide si participar; por su parte, el albergue gestiona la llegada de voluntarios sin coordinación estructurada.

### Problemas detectados
- No existe validación formal de disponibilidad de cupos.  
- Falta de comunicación estructurada entre voluntario, coordinación y albergue.  
- El flujo carece de trazabilidad.  
- El proceso es manual y depende de comunicación informal.

---

## 3. TO-BE: Propuesta de Rediseño

El proceso fue reorganizado en tres flujos independientes, uno por actor, para otorgar claridad, orden y responsabilidad en cada etapa.  
Cada actor ejecuta únicamente las tareas que le corresponden y el proceso incorpora validaciones, decisiones y manejo de excepciones.

### 3.1 TO-BE Voluntario
El voluntario:
- Accede al portal,
- Ingresa datos y preferencias,
- Revisa sugerencias disponibles,
- Decide si aceptar o no la recomendación,
- Envía su solicitud,
- Recibe una confirmación de inscripción.

### 3.2 TO-BE Administrador / Coordinador
El administrador:
- Revisa solicitudes recibidas,
- Consulta necesidades vigentes,
- Verifica disponibilidad de cupos,
- Asigna voluntarios cuando es posible,
- Registra la asignación,
- Envía la confirmación correspondiente,
- En caso de no haber cupos, registra la solicitud en lista de espera.

### 3.3 TO-BE Albergue
El albergue:
- Recibe solicitud de confirmación,
- Revisa requisitos y disponibilidad logística,
- Decide si puede recibir al voluntario,
- Confirma disponibilidad o rechaza la solicitud,
- Envía la respuesta final.

---

## 4. Heurísticas de Rediseño Aplicadas
- Resequencing / Knock-out: validar disponibilidad antes de continuar.  
- Parallelism acotado: algunas acciones pueden ocurrir sin retrasar el flujo principal.  
- Contact Reduction: se reduce la cantidad de pasos innecesarios.  
- Exception Handling: se contemplan situaciones sin cupos y decisiones de rechazo.

---

## 5. Impacto del Rediseño (Devil’s Quadrangle)

| Criterio     | Impacto | Justificación |
|--------------|---------|---------------|
| Tiempo       | Disminuye | Flujo más ordenado y validaciones tempranas. |
| Costo        | Disminuye | Menos retrabajo y reducción de pasos manuales. |
| Calidad      | Aumenta | Estructura clara, mejor control de asignaciones y respuestas. |
| Flexibilidad | Se mantiene | El proceso permite manejar excepciones sin perder coherencia. |

---

## 6. Conclusión

El rediseño del Proceso de Voluntariado ofrece un flujo más claro, eficiente y trazable.  
La separación por actores mejora la organización, reduce tiempos y permite una gestión coherente desde la inscripción del voluntario hasta la confirmación final por parte del albergue.

Se incluyen los tres diagramas TO-BE:
- TO-BE Voluntario  
- TO-BE Administrador / Coordinador  
- TO-BE Albergue  

