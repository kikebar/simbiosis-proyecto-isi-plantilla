# Requisitos

Esta carpeta contiene la especificación de requisitos de Proyecto Simbiosis.

La línea base de requisitos está formada por los dos documentos siguientes, que deben versionarse y publicarse conjuntamente:

- **[Especificación de requisitos de software (SRS)](srs.md):** describe el propósito, alcance, contexto, interfaces, atributos de calidad, decisiones abiertas, glosario, modelos y trazabilidad del producto.
- **[Catálogo de requisitos](catalogo-requisitos.md):** contiene el texto canónico de los requisitos de usuario (UR), funcionales (FR) y no funcionales (NFR), junto con sus identificadores, fuentes, estado y relaciones de trazabilidad.

El catálogo no es una especificación independiente: es parte de la SRS. Para consultar o aprobar una versión de la especificación se deben utilizar siempre ambos documentos en la misma versión o etiqueta de publicación.

## Relación entre documentos

La SRS y el catálogo establecen los requisitos de referencia. Las historias de búsqueda desarrollan las necesidades de UR-08 y UC-21, conforme al acta de acuerdos de búsqueda. Cada historia conserva sus fuentes y sus criterios de aceptación.

La épica reúne la necesidad conjunta. Su división y las decisiones de revisión se documentan junto a las historias.

## Convenciones

- Los identificadores de requisitos son estables y no se reutilizan.
- El catálogo es la única fuente de verdad para la redacción atómica de UR, FR y NFR.
- El glosario forma parte de la SRS.
- Las decisiones de captura posteriores que precisen información del Documento de Visión y Alcance se registran en las actas correspondientes y se reflejan en esta línea base con su trazabilidad.
- Las solicitudes de cambio aprobadas actualizan los documentos afectados y quedan registradas en [`../cambios/`](../cambios/registro-solicitudes-cambio.md).

## Documentación relacionada

- [Plantilla de backlog](plantilla-backlog.md), v1.2. Estructura vacía para preparar `backlog-propuesto.md`: orden, decisiones de prioridad, comprobaciones de calidad y Definición de Hecho. La posición y el identificador de cada historia son independientes. La conclusión vincula una condición de DoD con la evidencia necesaria.
- [Historias de usuario de búsqueda](historias-usuario-busqueda.md), v1.2, Revisado. Épica descompuesta en US-01, US-02 y US-03, con criterios de aceptación, fuentes y justificación de la división.
- [Visión y alcance](../vision/vision_y_alcance.md)
- [Actas de captura y aclaraciones](../captura/README.md)
- [Registro de decisiones](../decisiones/registro-decisiones.md)
- [Criterios de revisión de requisitos](../calidad/criterios-revision-requisitos.md)
- [Modelos de análisis](../modelos/README.md)
- [Plantilla de historias de usuario de búsqueda](plantilla-historias-usuario-busqueda.md), v1.2. Estructura reutilizable para documentar la épica de búsqueda, su división en US-01 a US-03, los criterios de aceptación, las fuentes y las decisiones de revisión. El documento resultante se mantiene en `historias-usuario-busqueda.md`.
