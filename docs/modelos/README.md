# Modelos

Modelos y diagramas propios del Proyecto Simbiosis (por ejemplo, modelos de dominio, de procesos o de datos) que apoyan la comprensión de los requisitos.

## Contenido

| Documento | Finalidad |
| --- | --- |
| [Plantilla del modelo de casos de uso](plantilla-modelo-casos-de-uso.md) | Estructura e instrucciones reutilizables, que se conservan sin cumplimentar. |
| [Modelo de casos de uso](modelo-casos-de-uso.md) | Documento de trabajo que incorpora los resultados de E1 y se amplía y revisa en las iteraciones siguientes. |

Cada modelo nuevo debe añadirse a esta carpeta en Markdown (o como diagrama embebido en Markdown) y listarse en la tabla anterior.

## Nombres de las imágenes

Guarda las imágenes de los diagramas en `docs/modelos/imagenes/`. Utiliza este patrón:

```text
tipo-de-diagrama-ambito.png
```

El tipo identifica el diagrama. El ámbito identifica las funciones, el escenario o los elementos representados. Utiliza minúsculas, sin tildes, eñes ni espacios. Separa las palabras con guiones. No añadas el nombre del estudiante, el código de la práctica, la fecha ni un número de versión. Las vistas de E1 y E2 añaden el sufijo de la iteración al ámbito, conforme a los nombres siguientes.

Para los diagramas de casos de uso, el tipo es `casos-de-uso`. El nombre común de la primera vista de E1 es `casos-de-uso-acceso-cuentas-ayuda-e1.png`.

| Imagen | Nombre |
| --- | --- |
| Vista de acceso, cuentas y ayuda de E1 | `casos-de-uso-acceso-cuentas-ayuda-e1.png` |
| Vista de salud y recetas de E2 | `casos-de-uso-salud-recetas-e2.png` |
| Vista separada de actores del ámbito de E1, si se necesita | `casos-de-uso-acceso-cuentas-ayuda-actores-e1.png` |

Si necesitas más de una imagen para el mismo tipo y ámbito, añade un detalle descriptivo al final. No uses nombres como `imagen1`, `diagrama-final` o `copia-2`. El detalle debe explicar qué distingue esa imagen. No es necesario dividir una vista para utilizar ese sufijo.

Cuando revises una vista, actualiza el archivo con el mismo nombre. Cuando añadas una vista con otro alcance, crea un archivo con otro ámbito. Git conservará los estados anteriores que hayas registrado en commits.

El formato habitual de las imágenes es PNG. Si una actividad admite otro formato, conserva el mismo nombre base y cambia solo la extensión. Un archivo editable de la herramienta utiliza también ese nombre base y su extensión propia.

La convención se ampliará en esta guía cuando se incorporen otros tipos de diagramas. Por ejemplo, podrá usar los tipos `clases`, `secuencia` o `actividad`, seguidos del ámbito correspondiente. Estos ejemplos no establecen tareas para las próximas prácticas.

Los documentos Markdown utilizan enlaces relativos. Desde un archivo situado directamente en `docs/modelos/`, el enlace a una imagen comienza por `imagenes/`.

## Uso de la plantilla base

La plantilla base se conserva en `plantilla-modelo-casos-de-uso.md`. Para iniciar un modelo, copia su contenido en `modelo-casos-de-uso.md` y completa ese documento. El modelo del repositorio contiene el resultado revisado de E1: actores, casos, diagrama y respaldo en los requisitos. La revisión v1.5 descompone UC-08 en cinco casos. Las descripciones detalladas quedan pendientes.

La imagen de esta referencia se conserva como `imagenes/casos-de-uso-acceso-cuentas-ayuda-e1.png`. El nombre se utiliza también para el trabajo del alumnado. La vista de E2 sigue el mismo criterio: `casos-de-uso-salud-recetas-e2.png`.

Una vez iniciado el modelado, continúa sobre el documento de trabajo. No vuelvas a copiar la plantilla sobre un modelo que ya contiene resultados. Consulta la plantilla cuando necesites sus instrucciones o el esquema de un apartado. Las mejoras de la estructura o las instrucciones se realizan en la plantilla; los actores, casos, diagramas y resultados del proyecto se incorporan al modelo.

## Versionado del modelo de casos de uso

El modelo mantiene una ruta estable: `modelo-casos-de-uso.md`. Cada iteración amplía o revisa ese archivo. No se crean copias del documento con nombres como E1, E2 o «versión anterior».

Los commits conservan los estados registrados del documento. Conservan también las imágenes y los archivos editables que se hayan incluido en esos commits. Para recuperar una vista anterior, consulta esos archivos en el mismo commit. Un enlace a una imagen externa que cambia no conserva su contenido dentro de Git.

Durante una iteración puede haber varios commits. Al cerrarla, identifica el commit que contiene el estado revisado y registra su referencia en la evaluación de esa iteración. Por ejemplo, el estado de cierre de E1 se localizará mediante esa referencia, aunque el archivo se siga modificando en E2.

La versión visible del documento, la iteración y el commit indican cosas diferentes. La versión identifica una revisión del documento. La iteración sitúa esa revisión en el proceso. El commit permite recuperar los archivos exactos. No es necesario cambiar la versión visible por cada corrección pequeña.

Si se declara una línea base formal, se identifica mediante una etiqueta de Git y una entrada en el [historial de líneas base](../../CHANGELOG.md), conforme a las convenciones del repositorio. Cerrar una iteración no declara automáticamente una línea base. Para el trabajo ordinario del modelo basta con identificar el commit correspondiente.
