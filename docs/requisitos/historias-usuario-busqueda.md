# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Versión | 1.3 |
| Estado | Revisado |

## Alcance y fuentes

Este documento descompone la búsqueda por texto, ingredientes incluidos e ingredientes excluidos en tres historias. No especifica UC-21 completo.

- [Catálogo de requisitos](catalogo-requisitos.md): UR-08; FR-085, FR-086, FR-087 y FR-102.
- [Acta de acuerdos de UC-21 Buscar recetas](../captura/acta-acuerdos-uc-21-buscar-recetas.md), v1.1, Vigente.

Los criterios de aceptación seleccionan situaciones que permiten comprobar cada capacidad. Los demás acuerdos del acta siguen vigentes.

## Contexto común

La persona tiene la sesión iniciada. Las búsquedas consideran recetas publicadas y validadas. Los resultados se ordenan por fecha de publicación, con las más recientes primero. Las vistas previas siguen lo acordado en el apartado [Resultados y detalle del acta](../captura/acta-acuerdos-uc-21-buscar-recetas.md#resultados-y-detalle).

La persona debe indicar al menos un criterio. Si no indica ninguno, el sistema solicita un criterio y conserva la búsqueda sin ejecutar. Un fallo de la consulta se comunica como un problema y no como una búsqueda sin resultados. El sistema conserva los criterios.

## Épica de búsqueda

Como usuario registrado, quiero buscar recetas con texto e ingredientes que deseo incluir o excluir, para encontrar una receta que se ajuste a lo que quiero preparar.

**Estado:** descompuesta en US-01, US-02 y US-03. Conserva la necesidad conjunta y agrupa las tres historias.

## Justificación de la división

La división separa tres capacidades que aportan valor por sí mismas. Cada una produce resultados de búsqueda y puede combinarse con las otras mediante los acuerdos del acta. La épica es la agrupación; no se cuenta como una cuarta historia.

## US-01 · Buscar mediante una palabra o frase

Como usuario registrado, quiero buscar recetas mediante una palabra o frase, para localizar recetas relacionadas con lo que quiero preparar.

**Fuentes:** [catálogo](catalogo-requisitos.md), UR-08, FR-085 y FR-102; UC-21; acta, [Criterios de búsqueda](../captura/acta-acuerdos-uc-21-buscar-recetas.md#criterios-de-búsqueda) y [Búsqueda sin resultados](../captura/acta-acuerdos-uc-21-buscar-recetas.md#búsqueda-sin-resultados).

### Criterios de aceptación

- **CA-01.** Dada una receta publicada y validada con «calabacín» en su título, cuando la persona busca «CALABACIN», entonces esa receta aparece entre los resultados.
- **CA-02.** Dadas recetas con «arroz integral» en el título o la descripción breve y otras con las palabras separadas o en orden inverso, cuando la persona busca «arroz integral», entonces aparecen las primeras y no las otras. No se distinguen mayúsculas ni tildes.
- **CA-03.** Dado que ninguna receta cumple el texto indicado, cuando la persona ejecuta la búsqueda, entonces el sistema informa de que no hay resultados y conserva los criterios. Las sugerencias disponibles se muestran aparte. No se modifican los criterios ni se ejecuta otra búsqueda sin una acción de la persona.

### Reglas relacionadas

Las sugerencias conservan las exclusiones. La persona ve los criterios propuestos y decide si ejecuta otra búsqueda. Si no hay sugerencias, el sistema lo indica.

### Revisión INVEST de US-01

| Criterio | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- |
| Independiente | Sí | Sí | Permite obtener recetas mediante una palabra o frase sin implementar antes la inclusión ni la exclusión de ingredientes. CA-01 y CA-02 muestran ese resultado útil; la historia puede compartir el catálogo de recetas y la infraestructura de búsqueda con las otras dos. |
| Negociable | Sí | Sí | Se puede acordar cómo introducir el texto y presentar los resultados y las sugerencias. Deben mantenerse las reglas del acta sobre los campos consultados, la coincidencia sin distinguir mayúsculas ni tildes, el orden de la frase y la ayuda sin cambiar los criterios ni ejecutar otra búsqueda sin una acción de la persona. |
| Valiosa | Sí | Sí | Permite a la persona localizar recetas relacionadas con lo que quiere preparar a partir de una palabra o frase. Obtiene resultados de búsqueda que puede valorar, sin tener que conocer ni seleccionar previamente los ingredientes de esas recetas. |
| Estimable | Sí | Sí | La historia, CA-01–03 y el acta delimitan la búsqueda en título o descripción breve, la coincidencia del texto y la respuesta sin resultados. El trabajo que se estime debe incluir también las sugerencias acordadas; el equipo debe valorar su solución técnica y aclarar cualquier incertidumbre que impida estimarla. |
| Pequeña | Sí | Sí | Se centra en buscar por texto y responder cuando esa búsqueda no obtiene resultados; deja fuera la búsqueda por ingredientes, los demás filtros y la consulta del detalle. La ayuda con sugerencias forma parte del alcance y debe tenerse en cuenta al confirmar que el tamaño sea manejable para el equipo. |
| Comprobable | Sí | Sí | CA-01 permite detectar una búsqueda que distinga mayúsculas o tildes; CA-02, una que acepte palabras separadas o en orden inverso. CA-03 permite comprobar el aviso sin resultados y la conservación de los criterios; los acuerdos del acta completan las comprobaciones de las sugerencias. |

## US-02 · Buscar por ingredientes incluidos

Como usuario registrado, quiero buscar recetas que contengan los ingredientes que selecciono, para encontrar preparaciones que utilicen esos ingredientes.

**Fuentes:** [catálogo](catalogo-requisitos.md), UR-08 y FR-086; UC-21; acta, [Criterios de búsqueda](../captura/acta-acuerdos-uc-21-buscar-recetas.md#criterios-de-búsqueda).

### Criterios de aceptación

- **CA-01.** Dadas recetas con arroz y otras sin arroz, cuando la persona selecciona arroz y busca, entonces solo aparecen recetas que contienen arroz.
- **CA-02.** Dadas recetas con arroz y pollo, otras solo con arroz y otras solo con pollo, cuando la persona selecciona arroz y pollo y busca, entonces solo aparecen las que contienen ambos.
- **CA-03.** Dado que la persona ha seleccionado arroz y pollo, cuando retira pollo y ejecuta la búsqueda, entonces se buscan recetas con arroz y no se exige que contengan pollo.

### Reglas relacionadas

La persona selecciona nombres de ingredientes disponibles en el sistema. Una receta debe contener todos los ingredientes incluidos. Puede contener otros ingredientes. La búsqueda utiliza la selección actual.

### Revisión INVEST de US-02

| Criterio | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- |
| Independiente | Sí | Sí | Permite seleccionar ingredientes y obtener recetas que los contengan sin implementar antes la búsqueda por texto ni las exclusiones. CA-01 muestra una búsqueda solo por arroz; la capacidad incluye obtener los resultados y puede compartir infraestructura con las otras historias. |
| Negociable | Sí | Sí | Se puede acordar cómo presentar los ingredientes disponibles y cómo añadirlos o retirarlos de la selección. Debe mantenerse la regla del acta: cada resultado contiene todos los ingredientes seleccionados, aunque puede contener otros, y la búsqueda utiliza la selección actual. |
| Valiosa | Sí | Sí | Permite encontrar preparaciones que utilicen los ingredientes elegidos por la persona. Al exigir que cada receta los contenga todos, evita que tenga que revisar resultados que solo coinciden con una parte de su selección. |
| Estimable | Sí | Sí | La historia y CA-01–03 delimitan la selección de ingredientes disponibles, la búsqueda de recetas que los contienen todos y el cambio de resultados al retirar una selección. El acta precisa esas reglas, lo que permite identificar el trabajo que debe estimarse; arroz y pollo son datos de prueba, no un límite de dos ingredientes. |
| Pequeña | Sí | Sí | Se centra en una capacidad completa: seleccionar ingredientes y obtener recetas que los contengan. Añadir o retirar una selección ajusta esa misma búsqueda; quedan fuera gestionar el catálogo de ingredientes, buscar por texto, excluir ingredientes y consultar el detalle de una receta. |
| Comprobable | Sí | Sí | CA-01 distingue recetas con arroz de recetas sin él; CA-02 detecta si el sistema acepta solo uno de los ingredientes cuando se han elegido dos. CA-03 permite comprobar que retirar pollo elimina esa exigencia y que la búsqueda utiliza la selección actual. |

## US-03 · Excluir ingredientes

Como usuario registrado, quiero excluir ingredientes de una búsqueda, para evitar recetas que contengan ingredientes que no quiero utilizar.

**Fuentes:** [catálogo](catalogo-requisitos.md), UR-08 y FR-087; UC-21; acta, [Criterios de búsqueda](../captura/acta-acuerdos-uc-21-buscar-recetas.md#criterios-de-búsqueda).

### Criterios de aceptación

- **CA-01.** Dadas recetas con leche, con huevo, con ambos y sin ninguno, cuando la persona excluye leche y huevo y busca sin otros criterios, entonces solo aparecen recetas sin leche ni huevo.
- **CA-02.** Dadas recetas que cumplen distintas combinaciones, cuando la persona busca «arroz integral», incluye pollo y excluye leche, entonces cada resultado coincide con el texto, contiene pollo y no contiene leche.
- **CA-03.** Dado que arroz está seleccionado para incluirlo y excluirlo, cuando la persona intenta buscar, entonces el sistema señala el conflicto, conserva los criterios y no ejecuta la búsqueda hasta que la persona lo corrija.

### Reglas relacionadas

Excluir ingredientes es suficiente para ejecutar una búsqueda. Si se combinan capacidades, cada receta debe cumplir todos los criterios. Basta contener cualquiera de los ingredientes excluidos para quedar fuera. La exclusión expresa no activa un filtro del perfil ni garantiza seguridad frente a alergias.

### Revisión INVEST de US-03

| Criterio | Aplicado | Cumple | Justificación |
| --- | --- | --- | --- |
| Independiente | Sí | Sí | Permite obtener recetas utilizando solo ingredientes excluidos, sin implementar antes la búsqueda por texto ni la inclusión de ingredientes, como muestra CA-01. CA-02 y CA-03 comprueban la integración con las otras capacidades cuando están disponibles; esa integración debe planificarse, aunque la exclusión ya ofrece un resultado útil por separado. |
| Negociable | Sí | Sí | Se puede acordar cómo seleccionar y mostrar los ingredientes excluidos y cómo señalar un conflicto. Deben mantenerse las reglas del acta: ningún resultado contiene cualquiera de los ingredientes excluidos y, si uno está incluido y excluido a la vez, se conservan los criterios y no se ejecuta la búsqueda hasta corregirlo. |
| Valiosa | Sí | Sí | Permite evitar recetas que contengan ingredientes que la persona no quiere utilizar, incluso cuando solo indica exclusiones. El beneficio es ajustar los resultados a esa elección expresa; la historia no aplica automáticamente el perfil ni garantiza seguridad frente a alergias. |
| Estimable | Sí | Sí | La historia y CA-01–03 delimitan la exclusión por sí sola, su combinación con texto e inclusión y la detección de un ingrediente incluido y excluido a la vez. El acta fija el resultado de cada situación; la estimación debe contemplar también el trabajo de integración con las otras capacidades. |
| Pequeña | Sí | Sí | Se centra en excluir ingredientes y obtener resultados que respeten esa selección. La combinación y el conflicto comprueban cómo se incorpora la exclusión a la búsqueda; quedan fuera los filtros automáticos del perfil, la gestión de alergias y los demás filtros de UC-21. |
| Comprobable | Sí | Sí | CA-01 detecta si se admite alguna receta con leche o huevo cuando ambos están excluidos. CA-02 exige que cada resultado cumpla las tres condiciones de la búsqueda; CA-03 permite comprobar que un conflicto se señala, conserva los criterios y bloquea la ejecución hasta corregirlo. |

## Revisión de las historias con INVEST

Estimable y Pequeña son juicios razonados sobre el alcance descrito. El equipo que vaya a implementar las historias debe confirmar que conoce los datos y las condiciones técnicas necesarios y que el trabajo cabe en su capacidad disponible. Los criterios de aceptación aportan ejemplos de comprobación; no sustituyen los demás acuerdos del acta ni demuestran por sí solos el esfuerzo requerido.

Las tres historias expresan capacidades útiles por separado y un beneficio para la persona. Su alcance es comprensible y sus criterios permiten comprobar resultados. La redacción deja abierta la implementación. Pueden compartir infraestructura.

US-03 describe la capacidad de excluir ingredientes y su beneficio. El criterio con leche y huevo comprueba que ninguna receta contiene cualquiera de los ingredientes excluidos. La historia no impone una interfaz concreta.
