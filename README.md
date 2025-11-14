Rediseño TO-BE – Proceso de Voluntariado

Martin Araya Riquelme - 21.624.104-5 / Francisco Villagrán Madrid - 21.483.516-9 / Gladys Carvacho - 21.205.052-0

📘 Descripción General

El proyecto consiste en analizar y rediseñar un proceso real del sistema de albergues, aplicando buenas prácticas de Ingeniería de Procesos (AS-IS / TO-BE).
El proceso seleccionado es Voluntariado, que define cómo los voluntarios se informan, se inscriben y son asignados a un albergue.

Se desarrolla:

Un AS-IS que refleja el funcionamiento actual (simple, sin validaciones ni coordinación formal).

Un TO-BE con tres procesos separados:
Voluntario, Administrador/Coordinador y Albergue, siguiendo las indicaciones del profesor y eliminando agentes incorrectos como “Sistema de Ayuda”.

🔹 AS-IS: Situación Actual

Nombre: Proceso de Voluntariado (AS-IS)

Descripción:
El voluntario ingresa al portal, revisa la información disponible y decide si desea participar.
El albergue recibe voluntarios de manera manual y descoordinada, sin confirmaciones formales ni validaciones.

Problemas identificados

Falta de comunicación entre actores.

No hay validación de requisitos o cupos.

No existe trazabilidad ni registro formal.

La confirmación al voluntario depende de conversaciones informales.

🔹 TO-BE: Propuesta de Rediseño

El TO-BE se rediseñó siguiendo la rúbrica del profesor y separando claramente tres procesos independientes:

1️⃣ Proceso TO-BE Voluntario

El voluntario:

Accede al portal

Ingresa sus datos y preferencias

Revisa sugerencias

Decide si inscribirse

Envía la solicitud

Recibe la confirmación final

✔ Sin tareas redundantes
✔ Sin actor “sistema”
✔ Gateways exclusivos bien utilizados

2️⃣ Proceso TO-BE Administrador / Coordinador

El administrador:

Revisa solicitudes recibidas

Consulta necesidades vigentes

Verifica cupos disponibles

Asigna voluntarios cuando hay disponibilidad

Registra la asignación

Envia confirmación

Maneja excepción: lista de espera

✔ Gateway con dos salidas exclusivas (SI / NO)
✔ Diagrama no sobrecargado
✔ No se mezcla con funciones del albergue

3️⃣ Proceso TO-BE Albergue

El albergue:

Recibe la solicitud del administrador

Revisa requisitos y disponibilidad

Decide si puede recibir al voluntario

Confirma logística o rechaza

Envía la respuesta

✔ Gateway con condiciones SI/NO
✔ Sin “sistema de ayuda”
✔ Cierre limpio del proceso

🧠 Heurísticas de Rediseño Aplicadas
Heurística	Aplicación en el TO-BE
Resequencing / Knock-Out	Se verifica disponibilidad y requisitos antes de registrar al voluntario.
Parallelism	Algunas actividades pueden gestionarse sin detener el flujo (p. ej., registro vs. comunicación).
Contact Reduction	El voluntario recibe una confirmación final clara y única.
Exception Handling	Se implementó proceso para lista de espera y rechazo.
⚙️ Impacto del Rediseño (Devil’s Quadrangle)
Criterio	Impacto	Justificación
Tiempo	⬇️	Se elimina trabajo manual innecesario y se ordena el flujo.
Costo	⬇️	Menos retrabajo y menos pasos redundantes.
Calidad	⬆️	Confirmación clara, registro formal, trazabilidad.
Flexibilidad	≈	El proceso es más estructurado, pero sigue permitiendo manejo de casos especiales.
🏁 Conclusión

El rediseño logra transformar un proceso informal y fragmentado en una secuencia clara, trazable y estandarizada.
La separación en tres procesos TO-BE permite transparencia, control y alineación con la rúbrica del curso, asegurando que cada actor desempeñe solo las funciones que realmente le corresponden.
