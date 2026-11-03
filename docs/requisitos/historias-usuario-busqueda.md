# Historias de usuario de búsqueda

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Versión | 1.1 |
| Estado | Borrador |

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
| Independiente | Sí | Sí | La búsqueda por texto produce resultados sin seleccionar ingredientes. CA-01 y CA-02 muestran ese resultado. |
| Negociable | Sí | Sí | Pide localizar recetas; deja abierta la solución técnica. La coincidencia y la ayuda sin resultados respetan el acta. |
| Valiosa | Sí | Sí | El «para» explica el beneficio: localizar recetas relacionadas con lo que quiere preparar. |
| Estimable | Sí | Sí | CA-01–03 delimitan coincidencia, frase y respuesta sin resultados; el acta precisa los datos y reglas. |
| Pequeña | Sí | Sí | Se centra en buscar por palabra o frase. CA-03 trata el caso sin resultados de esa misma búsqueda. |
| Comprobable | Sí | Sí | CA-01 contrasta tildes y mayúsculas; CA-02, frase y orden; CA-03, ausencia de resultados y criterios conservados. |

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
| Independiente | Sí | Sí | CA-01 permite buscar solo por arroz, sin texto ni exclusiones. |
| Negociable | Sí | Sí | Pide recetas con ingredientes elegidos y no prescribe controles de interfaz. Respeta la regla del acta de incluirlos todos. |
| Valiosa | Sí | Sí | El «para» explica el beneficio: encontrar preparaciones que utilicen los ingredientes elegidos. |
| Estimable | Sí | Sí | CA-01–03 delimitan uno o dos ingredientes y el cambio de selección; el acta fija la regla de inclusión. |
| Pequeña | Sí | Sí | Se limita a incluir ingredientes en la búsqueda y obtener resultados; retirar uno actualiza la misma selección. |
| Comprobable | Sí | Sí | CA-01 separa recetas con y sin arroz; CA-02 exige ambos ingredientes; CA-03 comprueba la selección actual. |

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
| Independiente | Sí | Sí | CA-01 ejecuta una búsqueda solo con exclusiones, sin texto ni ingredientes incluidos. |
| Negociable | Sí | Sí | Pide evitar ingredientes seleccionados y deja abierta la interfaz. CA-03 respeta el acuerdo sobre el conflicto. |
| Valiosa | Sí | Sí | El «para» explica el beneficio: evitar recetas con ingredientes que no quiere utilizar. |
| Estimable | Sí | Sí | CA-01–03 delimitan exclusión sola, combinación y conflicto; el acta fija el comportamiento acordado. |
| Pequeña | Sí | Sí | Se centra en excluir ingredientes. CA-02 comprueba que esa capacidad se combina con las demás. |
| Comprobable | Sí | Sí | CA-01 excluye leche y huevo; CA-02 exige las tres condiciones; CA-03 impide ejecutar criterios en conflicto. |

## Revisión de las historias con INVEST

Las tres historias expresan capacidades útiles por separado y un beneficio para la persona. Su alcance es comprensible y sus criterios permiten comprobar resultados. La redacción deja abierta la implementación. Pueden compartir infraestructura.

US-03 describe la capacidad de excluir ingredientes y su beneficio. El criterio con leche y huevo comprueba que ninguna receta contiene cualquiera de los ingredientes excluidos. La historia no impone una interfaz concreta.
