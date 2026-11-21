# Acta de acuerdos de UC-05 · Actualizar perfil

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Caso de uso | UC-05 · Actualizar perfil |
| Estado | En revisión; aclaraciones iniciales aprobadas |
| Versión | 1.2 |
| Fecha de redacción | 10/10/2026 |
| Aprobación inicial | 10/10/2026 |
| Revisión de preferencias dietéticas | 19/11/2026; SC-002 |
| Tipo | Acta simulada de aclaración |
| Finalidad | Concretar el comportamiento de UC-05. |

Esta acta recoge las respuestas que el analista habría obtenido al consultar a una persona usuaria. No documenta una entrevista real. Las aclaraciones iniciales fueron aprobadas el 10/10/2026. La revisión posterior limita las preferencias dietéticas a pacientes, conforme a SC-002. Complementan el catálogo canónico para el alcance seleccionado; no modifican su redacción.

## 1. Participantes y alcance

En la simulación participan un analista y una persona usuaria registrada. La persona quiere actualizar su propio perfil y conservar los cambios.

La consulta se centra en datos personales, datos de contacto y preferencias dietéticas. La persona ya tiene una cuenta activa y una sesión iniciada. El registro, el inicio de sesión, el cambio de contraseña y la eliminación de la cuenta quedan fuera de esta consulta.

## 2. Acuerdos

### Datos que se pueden modificar

- La persona puede consultar los valores guardados antes de modificarlos.
- Para esta descripción se consideran el nombre completo, el teléfono y la dirección postal. Si la persona tiene perfil de paciente, también se consideran sus preferencias dietéticas.
- El alias y el correo electrónico se muestran como datos de consulta. No se pueden modificar, conforme a FR-019.
- El nombre completo y el teléfono siguen siendo obligatorios. La dirección postal es opcional.
- Las preferencias dietéticas son opcionales y corresponden exclusivamente a pacientes. Un paciente puede seleccionar ninguna, una o varias: vegana, sin gluten y baja en carbohidratos. Los usuarios sin perfil de paciente no pueden seleccionarlas ni editarlas.
- Las preferencias no son datos de salud ni sustituyen el registro de alergias. Esta consulta no modifica datos de salud.

### Validación de los cambios

- El nombre completo y el teléfono no pueden quedar vacíos. Un valor formado solo por espacios se considera vacío.
- El teléfono conserva las reglas de formato del registro, incluidos los prefijos internacionales.
- Si un dato no es válido, el sistema identifica el campo y explica qué debe corregirse. Conserva los valores introducidos y no guarda ningún cambio.
- La persona puede corregir los datos y volver a solicitar el guardado.

### Guardado y cancelación

- La edición no cambia por sí sola los datos guardados. La persona debe solicitar el guardado.
- Cuando los datos son válidos, el sistema guarda conjuntamente los cambios y confirma que el perfil se ha actualizado.
- Si la persona cancela antes de guardar, se descartan los cambios de esa edición. El perfil conserva los valores anteriores.
- Si el sistema no puede guardar, informa del problema y no confirma la actualización. Conserva los valores introducidos para que la persona pueda reintentar el guardado. Los datos guardados permanecen sin cambios.

## 3. Fuentes y relación con los requisitos

| Fuente | Respaldo |
| --- | --- |
| [Catálogo canónico de requisitos](../requisitos/catalogo-requisitos.md), UR-03, FR-019 y FR-220 | Actualización de información personal y preferencias; exclusión del alias y del correo electrónico. |
| [Acta general de captura](acta-captura-requisitos-generales.md), apartado 1.1 | Datos obligatorios y opcionales de la cuenta. |
| [Acta de UR-01](acta-captura-requisitos-ur-01.md), apartado 2.1 | Teléfono obligatorio y admisión de prefijos internacionales. |

La selección de campos para esta descripción, las opciones de preferencias y las respuestas ante validación, cancelación y fallo de guardado son concreciones aprobadas inicialmente, revisadas mediante [SC-002](../cambios/registro-solicitudes-cambio.md#solicitudes) para limitar las preferencias dietéticas a pacientes. No eliminan otras posibilidades de edición cubiertas por FR-019.
