# Acta de acuerdos sobre la información del dominio

| Campo | Valor |
| --- | --- |
| Proyecto | Proyecto Simbiosis |
| Estado | Cerrada; alcance acotado y cuestiones pendientes |
| Versión | 1.0 |
| Fecha de preparación | 21/11/2026 |
| Fecha de cierre | 24/11/2026 |
| Alcance de esta versión | Gestión de usuarios, recetas, foro, datos de salud, publicaciones de salud, moderación de contenidos y guía interactiva |
| Finalidad | Reunir y precisar la información del dominio necesaria para su análisis conceptual. |

Esta acta organiza la información de dominio de los módulos analizados e incorpora aclaraciones confirmadas durante sus revisiones documentales del 19 y el 21/11/2026. No documenta una nueva entrevista. Los apartados 2 a 8 organizan la información por módulos. Los apartados 9 y 10 reúnen los acuerdos, los aspectos aplazados y las fuentes de cada módulo. El cierre del acta no convierte las propuestas provisionales en acuerdos ni resuelve las cuestiones pendientes de aclaración con el cliente.

## Índice

- [1 Objeto y alcance](#1-objeto-y-alcance)
- [2 Información del dominio: Gestión de usuarios](#2-información-del-dominio-gestión-de-usuarios)
  - [2.1 Identidad y cuenta](#21-identidad-y-cuenta)
  - [2.2 Perfiles y participación](#22-perfiles-y-participación)
  - [2.3 Relaciones de cuidado](#23-relaciones-de-cuidado)
  - [2.4 Acreditación profesional](#24-acreditación-profesional)
  - [2.5 Aprobación y administración de cuentas](#25-aprobación-y-administración-de-cuentas)
- [3 Información del dominio: Gestión de recetas](#3-información-del-dominio-gestión-de-recetas)
  - [3.1 Recetas e ingredientes](#31-recetas-e-ingredientes)
  - [3.2 Autoría y validación](#32-autoría-y-validación)
  - [3.3 Comentarios y valoraciones](#33-comentarios-y-valoraciones)
- [4 Información del dominio: Foro](#4-información-del-dominio-foro)
  - [4.1 Hilos, comentarios y autoría](#41-hilos-comentarios-y-autoría)
  - [4.2 Seguimiento y «me gusta»](#42-seguimiento-y-me-gusta)
  - [4.3 Moderación y límites](#43-moderación-y-límites)
- [5 Información del dominio: Gestión de datos de salud](#5-información-del-dominio-gestión-de-datos-de-salud)
  - [5.1 Historial y registros](#51-historial-y-registros)
  - [5.2 Mediciones fisiológicas](#52-mediciones-fisiológicas)
  - [5.3 Resultados de laboratorio y notas](#53-resultados-de-laboratorio-y-notas)
- [6 Información del dominio: Gestión de publicaciones de salud](#6-información-del-dominio-gestión-de-publicaciones-de-salud)
  - [6.1 Publicaciones y autoría](#61-publicaciones-y-autoría)
  - [6.2 Clasificación y recursos](#62-clasificación-y-recursos)
  - [6.3 Participación de usuarios](#63-participación-de-usuarios)
- [7 Información del dominio: Moderación de contenidos](#7-información-del-dominio-moderación-de-contenidos)
  - [7.1 Reportes y contenido reportable](#71-reportes-y-contenido-reportable)
  - [7.2 Actuaciones y apelaciones](#72-actuaciones-y-apelaciones)
  - [7.3 Expresiones prohibidas](#73-expresiones-prohibidas)
- [8 Información del dominio: Guía interactiva](#8-información-del-dominio-guía-interactiva)
  - [8.1 Guía, temas y pasos](#81-guía-temas-y-pasos)
  - [8.2 Tutoriales y progreso](#82-tutoriales-y-progreso)
- [9 Acuerdos de esta revisión y aspectos aplazados](#9-acuerdos-de-esta-revisión-y-aspectos-aplazados)
  - [9.1 Gestión de usuarios](#91-gestión-de-usuarios)
  - [9.2 Gestión de recetas](#92-gestión-de-recetas)
  - [9.3 Gestión de publicaciones de salud](#93-gestión-de-publicaciones-de-salud)
  - [9.4 Moderación de contenidos](#94-moderación-de-contenidos)
  - [9.5 Foro](#95-foro)
  - [9.6 Gestión de datos de salud](#96-gestión-de-datos-de-salud)
  - [9.7 Guía interactiva](#97-guía-interactiva)
- [10 Fuentes y trazabilidad](#10-fuentes-y-trazabilidad)
  - [10.1 Gestión de usuarios](#101-gestión-de-usuarios)
  - [10.2 Gestión de recetas](#102-gestión-de-recetas)
  - [10.3 Gestión de publicaciones de salud](#103-gestión-de-publicaciones-de-salud)
  - [10.4 Moderación de contenidos](#104-moderación-de-contenidos)
  - [10.5 Foro](#105-foro)
  - [10.6 Gestión de datos de salud](#106-gestión-de-datos-de-salud)
  - [10.7 Guía interactiva](#107-guía-interactiva)
- [11 Revisión y continuidad](#11-revisión-y-continuidad)
- [12 Historial de versiones](#12-historial-de-versiones)

## 1 Objeto y alcance

La descripción comprende Gestión de usuarios y vistas de Gestión de recetas, Foro, Gestión de datos de salud, Gestión de publicaciones de salud, Moderación de contenidos y Guía interactiva, módulos definidos en el apartado 2.2 del [Documento de Visión y Alcance](../vision/vision_y_alcance.md).

Los apartados 2 a 8 describen los módulos analizados; las vistas y las aclaraciones siguen siendo parciales.

Los flujos de uso, las validaciones, los mecanismos de autenticación y el ciclo de vida detallado de las cuentas se mantienen en sus fuentes canónicas. Esta selección de información no modifica los requisitos del producto.

## 2 Información del dominio: Gestión de usuarios

Las afirmaciones de este apartado sintetizan los acuerdos existentes y las aclaraciones confirmadas en el apartado 9.1. Los aspectos aplazados se mantienen separados de los acuerdos. Los términos del dominio conservan el significado del [glosario de la SRS](../requisitos/srs.md#9-glosario).

### 2.1 Identidad y cuenta

- Las personas registradas en Simbiosis se denominan usuarios. Cada persona registrada dispone de una única cuenta personal, de uso individual, que no se comparte con otras personas.
- La información identificativa y de contacto del usuario comprende el nombre completo, el alias, el correo electrónico, el teléfono móvil, la dirección postal, la fecha de nacimiento y la fotografía de perfil.
- La dirección postal es opcional: cada usuario puede no tener ninguna o tener una. Una dirección puede ser compartida por varios usuarios y está asociada al menos a uno. De ella se conocen el nombre de la calle, el número, la población, el código postal y el municipio.
- Cada paciente puede seleccionar ninguna, una o varias preferencias dietéticas entre vegana, sin gluten y baja en carbohidratos. Cada preferencia tiene un nombre y puede ser seleccionada por ningún paciente, por uno o por varios. Las preferencias dietéticas corresponden exclusivamente a pacientes.
- Una cuenta puede disponer de una contraseña local. Se conserva la fecha y la hora en que se completó el registro.

### 2.2 Perfiles y participación

- En esta descripción, cada usuario tiene al menos uno de los siguientes perfiles: paciente, cuidador, nutricionista o coordinador. No se consideran otros tipos de usuario.
- Una misma persona puede reunir varios de los cuatro perfiles. Cada perfil conserva sus condiciones de habilitación: disponer de un perfil no exime de cumplir las condiciones de los demás.
- Los perfiles de cuidador y nutricionista requieren aprobación del coordinador. El perfil de paciente no requiere esa aprobación adicional.
- En esta descripción se consideran los perfiles de cuidador y nutricionista ya habilitados. Cada uno tiene un único coordinador que aprobó su perfil; un coordinador puede aprobar ninguno o varios perfiles de cada tipo.

### 2.3 Relaciones de cuidado

- Un cuidador puede no tener pacientes a su cuidado o cuidar a uno o varios. Un paciente puede no tener cuidador o tener uno solo con relación de cuidado activa.
- Las relaciones de cuidado consideradas en esta descripción son las aceptadas por el paciente y vigentes.
- Para habilitar el perfil de cuidador debe existir al menos una relación de cuidado aceptada por un paciente. Después de habilitarse, el cuidador puede quedar temporalmente sin pacientes asociados.
- La aceptación de la relación de cuidado por el paciente y la aprobación de la cuenta de cuidador por el coordinador son condiciones diferentes.

### 2.4 Acreditación profesional

- Cada nutricionista aporta una documentación profesional. Cada documentación corresponde a un único nutricionista.
- La aprobación corresponde al coordinador y es necesaria para habilitar el perfil profesional.

### 2.5 Aprobación y administración de cuentas

- Se conoce el estado de cada cuenta. Cuando existe un bloqueo temporal, también se conoce su duración.
- En esta descripción se consideran las aprobaciones, suspensiones y eliminaciones de cuentas realizadas por el coordinador, que quedan registradas en un historial de auditoría. Las aprobaciones corresponden a cuentas cuyo titular solicita el perfil de cuidador o de nutricionista, o ambos perfiles.
- De cada actuación registrada se conservan la fecha, la hora y la acción realizada. Cada actuación es realizada por un único coordinador sobre una única cuenta. Una cuenta y un coordinador pueden estar asociados a ninguna, una o varias actuaciones.
- Al eliminar una cuenta, sus actuaciones permanecen en el historial, aunque dejan de estar asociadas a ella. No se conserva una copia del alias para identificar la cuenta afectada. En esta descripción no se contempla la eliminación de cuentas de coordinador.
- Las actuaciones registradas pertenecen a un historial de auditoría: cada actuación pertenece a un único historial, que puede contener ninguna o varias. Las actuaciones no se comparten entre historiales y, si se elimina un historial, se eliminan las actuaciones que lo integran.

## 3 Información del dominio: Gestión de recetas

Esta descripción comprende las recetas, sus ingredientes, autoría, validación, comentarios y valoraciones. Se consideran los contenidos con su autor asociado; los casos en que una eliminación de cuenta deje contenido sin autor asociado quedan fuera de esta vista. Las estadísticas y otras interacciones no se desarrollan en esta vista; sus requisitos siguen vigentes. Las cuestiones no resueltas se indican en el apartado 9.2.

### 3.1 Recetas e ingredientes

- Para publicar una receta se indican su título, sus ingredientes, las instrucciones de preparación, el tiempo de cocción y el número de porciones.
- Una receta contiene al menos un ingrediente y cada ingrediente aparece como máximo una vez en ella. Cada ingrediente tiene un nombre y puede aparecer en ninguna, una o varias recetas. Para cada ingrediente de una receta se indica la cantidad y su unidad.
- Una receta puede incluir ninguna, una o varias imágenes y ningún, uno o varios vídeos. Cada imagen y cada vídeo se asocian a un único contenido: una receta o una publicación de salud. Para las consultas de recetas se contempla también una descripción breve.

### 3.2 Autoría y validación

- Cada receta tiene un único usuario autor; un usuario puede crear ninguna, una o varias recetas. Los pacientes y cuidadores pueden proponer recetas; estas quedan pendientes de validación hasta su revisión por un nutricionista.
- Una receta validada tiene un único nutricionista validador. Un nutricionista puede validar ninguna, una o varias recetas propuestas por pacientes o cuidadores, que se publican como validadas. También puede publicar directamente como validada una receta de su autoría, actuando como su validador.
- En esta vista no se contempla la eliminación de cuentas de cuidadores ni de nutricionistas, aunque reúnan otros perfiles.

### 3.3 Comentarios y valoraciones

- Los usuarios pueden comentar recetas. Cada comentario corresponde a una única receta y tiene un único autor; una receta puede tener ningún comentario, uno o varios, y un usuario puede escribir ninguno, uno o varios comentarios. De cada comentario se conocen su texto, su fecha y su hora. Los comentarios de recetas son distintos de las publicaciones y comentarios del foro.
- Los usuarios pueden responder a comentarios de otros usuarios en recetas. Una respuesta es también un comentario y, al crearse, corresponde a un único comentario de la misma receta al que responde. Un comentario puede recibir ninguna, una o varias respuestas.
- Los usuarios pueden valorar recetas con una puntuación de una a cinco estrellas. Cada valoración corresponde a una única receta y tiene un único autor; una receta puede tener ninguna valoración, una o varias, y un usuario puede emitir ninguna, una o varias valoraciones. De cada valoración se conocen la puntuación, la fecha y la hora. Un usuario puede emitir como máximo una valoración por receta.
- Si se elimina un comentario, sus respuestas se conservan en la receta, pero dejan de estar asociadas al comentario eliminado. Si se elimina una receta, se eliminan sus comentarios y valoraciones.

## 4 Información del dominio: Foro

Esta descripción comprende los hilos, comentarios, respuestas, seguimiento y «me gusta» del foro. Los acuerdos, propuestas y aspectos aplazados se recogen en el apartado 9.5.

### 4.1 Hilos, comentarios y autoría

- El foro es un espacio común de intercambio. Cualquier persona puede consultarlo; para crear hilos o participar es necesario iniciar sesión. Los pacientes, cuidadores, nutricionistas y coordinadores pueden participar como usuarios.
- En esta descripción, el hilo constituye la publicación inicial y tiene título, cuerpo, fecha y hora de publicación. Cada hilo tiene un único usuario autor.
- Los usuarios pueden publicar comentarios en los hilos. Cada comentario pertenece a un único hilo y tiene un único usuario autor, texto, fecha y hora de publicación. Su texto tiene un límite de 1.000 caracteres.
- Una respuesta es un comentario que responde a otro comentario del mismo hilo. Un comentario puede recibir ninguna o varias respuestas y estas pueden responderse a cualquier profundidad.
- Si se elimina un hilo, se eliminan todos sus comentarios, incluidas las respuestas.
- En el foro se muestra el alias como identidad visible del usuario. Los comentarios del foro son distintos de los comentarios de recetas.

### 4.2 Seguimiento y «me gusta»

- Los usuarios pueden seguir hilos y consultar los que siguen en su perfil.
- Los hilos y los comentarios, incluidas las respuestas, pueden recibir «me gusta». Un usuario puede dar como máximo un «me gusta» a un mismo contenido y puede retirarlo.
- Se muestra el total de «me gusta» por publicación. Para identificar las publicaciones destacadas se consideran los «me gusta» recibidos en las últimas 24 horas; para este análisis se contempla conocer la fecha y la hora de cada «me gusta».

### 4.3 Moderación y límites

- El coordinador administra y modera el foro. Su contenido puede reportarse y los hilos y comentarios se revisan antes de su publicación frente a una lista de expresiones prohibidas, según el apartado 7.
- En esta vista no se contempla la eliminación de cuentas de cuidadores ni de nutricionistas, aunque reúnan otros perfiles, ni otros casos en que una eliminación de cuenta deje contenido sin autor asociado. Los requisitos de conservación siguen vigentes.
- La eliminación de comentarios y el tratamiento de las respuestas se recogen como propuesta pendiente de contraste en el apartado 9.5.

## 5 Información del dominio: Gestión de datos de salud

Esta descripción comprende el historial del paciente, las mediciones fisiológicas, los resultados de laboratorio y las notas de salud. Los acuerdos y aspectos aplazados figuran en el apartado 9.6.

### 5.1 Historial y registros

- Cada paciente tiene un único historial de salud y cada historial pertenece a un único paciente. El historial puede estar vacío: incorporar datos depende del paciente.
- El historial puede contener ninguna o varias mediciones fisiológicas, resultados de laboratorio y notas de salud. Cada registro pertenece a un único historial. Si se elimina un historial, se eliminan sus mediciones, resultados y notas.

### 5.2 Mediciones fisiológicas

- El paciente puede registrar peso, altura, presión arterial, frecuencia cardíaca y temperatura corporal. De cada medición se conocen su tipo, fecha y hora; la fecha y la hora pueden corresponder a una medición anterior a su introducción.
- En una medición de presión arterial se registran los valores sistólico y diastólico. En las demás mediciones de esta vista se registra un valor.

### 5.3 Resultados de laboratorio y notas

- Un resultado de laboratorio comprende el parámetro, un valor numérico, su unidad obligatoria y la fecha y hora. Puede incluir una nota breve de contexto. Entre los parámetros se encuentran la glucosa, el colesterol y otros configurables.
- Una nota de salud recoge texto libre sobre síntomas o estado diario, con un máximo de 500 caracteres. En esta vista se asocia a la fecha del día al que corresponde.

## 6 Información del dominio: Gestión de publicaciones de salud

Esta descripción reúne información sobre los consejos de vida saludable, denominados publicaciones de salud, y su relación con las personas usuarias y los recursos. Las aclaraciones pendientes figuran en el apartado 9.3.

### 6.1 Publicaciones y autoría

- Los nutricionistas verificados crean y publican consejos o artículos breves sobre alimentación y hábitos de vida saludables. Cada publicación tiene un único nutricionista autor, que puede crear ninguna, una o varias publicaciones. Los consejos se dirigen a pacientes y cuidadores; los nutricionistas también pueden acceder a ellos.
- Cada publicación tiene un título y un texto. Puede tener una publicación programada para una fecha y hora futuras.
- Del nutricionista autor se conocen su nombre completo, su especialidad médica y una breve biografía profesional, que se muestran con el consejo.

### 6.2 Clasificación y recursos

- Un consejo puede tener ninguna, una o varias categorías predefinidas —nutrición, ejercicio, salud mental y hábitos de sueño— y etiquetas expresadas mediante palabras clave. Cada categoría y cada etiqueta pueden asociarse a ninguna, una o varias publicaciones.
- Un consejo puede incluir ninguna, una o varias imágenes, vídeos, documentos PDF, recursos de audio y referencias o enlaces a estudios científicos o fuentes confiables. De cada referencia se conoce su contenido, que puede expresar una cita o un enlace. Una referencia puede asociarse a ninguna, una o varias publicaciones.
- Cada imagen y cada vídeo se asocian a un único contenido: una receta o una publicación de salud. Cada documento PDF y cada recurso de audio pertenecen a una única publicación de salud.

### 6.3 Participación de usuarios

- Las publicaciones de salud pueden leerse y comentarse. No reciben valoraciones numéricas.
- Cada comentario tiene texto, fecha, hora, un único usuario autor y corresponde a una única publicación. Un usuario puede escribir ningún comentario, uno o varios; una publicación puede tener ningún comentario, uno o varios.
- Se conoce el número de visualizaciones y de «me gusta» recibidos por cada consejo.

## 7 Información del dominio: Moderación de contenidos

Esta vista comprende reportes, actuaciones de moderación, apelaciones y expresiones prohibidas. Las concreciones propuestas y los aspectos aplazados figuran en el apartado 9.4.

### 7.1 Reportes y contenido reportable

- Un usuario registrado puede presentar ninguno o varios reportes. Cada reporte tiene un único usuario autor, una categoría, un contenido reportado, una fecha y una hora; puede incluir un comentario adicional. Un contenido puede recibir ningún reporte, uno o varios.
- Una categoría tiene un nombre y puede corresponder a ningún reporte, uno o varios. Entre las categorías de reporte se encuentran spam, contenido ofensivo, información errónea y lenguaje inapropiado.
- En esta vista pueden reportarse recetas, publicaciones de salud, comentarios de recetas y comentarios de publicaciones de salud. El contenido del foro también puede reportarse. Estos elementos se consideran contenido reportable.
- Un reporte puede estar pendiente o tener una resolución final. Un reporte pendiente no tiene coordinador que lo haya resuelto; un reporte resuelto tiene uno solo. Un coordinador puede resolver ninguno, uno o varios reportes.

### 7.2 Actuaciones y apelaciones

- El coordinador puede aprobar, editar, eliminar, mantener o restaurar contenido. Cada actuación de moderación registrada tiene una fecha, un detalle y un único coordinador responsable, y afecta a un único contenido. Un coordinador o un contenido pueden estar relacionados con ninguna actuación, una o varias.
- Una actuación puede estar relacionada con un reporte o no estarlo. Un reporte puede estar relacionado con ninguna actuación, una o varias. Las actuaciones quedan registradas para auditoría.
- Un usuario cuyo contenido haya sido eliminado puede presentar una apelación de esa decisión. En esta propuesta, cada apelación tiene un único usuario autor y corresponde a una actuación de eliminación; un usuario o una eliminación pueden tener ninguna apelación, una o varias.

### 7.3 Expresiones prohibidas

- Los coordinadores mantienen una lista editable de palabras o frases prohibidas, utilizadas para revisar antes de su publicación los hilos y comentarios. De cada expresión se conoce su texto. Una lista puede contener ninguna o varias expresiones y cada expresión pertenece a una única lista. Si se elimina una lista, se eliminan las expresiones que la integran. En esta propuesta, un coordinador puede mantener ninguna o varias listas y una lista puede ser mantenida por ningún coordinador o por varios.

## 8 Información del dominio: Guía interactiva

Esta descripción comprende los temas, pasos, tutoriales multimedia y progreso de la guía. Los acuerdos y aspectos aplazados figuran en el apartado 9.7.

### 8.1 Guía, temas y pasos

- La plataforma dispone de una guía interactiva con temas de ayuda sobre sus funcionalidades. En esta descripción se considera una única guía y se conoce su título; también se conoce el título de cada tema.
- Una guía contiene uno o varios temas. Un tema puede estar asociado a una única guía o quedar temporalmente sin guía; si se elimina una guía, sus temas pueden conservarse para incorporarlos a otra.
- Cada tema comprende uno o varios pasos y cada paso pertenece a un único tema. Los pasos tienen un número de orden y un texto; dos pasos de un mismo tema no comparten número.
- Los pasos recogen instrucciones para utilizar las funcionalidades. El usuario puede navegar libremente entre temas y pausar, reanudar o abandonar la guía.

### 8.2 Tutoriales y progreso

- Un tema puede no tener tutoriales multimedia o tener varios; cada tutorial pertenece a un único tema. De cada tutorial se conocen su título y tipo, que puede ser vídeo o animación, entre otros. Al eliminar un tema se eliminan sus pasos y tutoriales.
- En esta descripción se considera el progreso de usuarios registrados. Cada usuario puede tener un único punto de reanudación para la guía; cada punto pertenece a un único usuario, señala un único paso y conserva la fecha de su última actualización. El tema se identifica a través del paso.

## 9 Acuerdos de esta revisión y aspectos aplazados

### 9.1 Gestión de usuarios

Las siguientes aclaraciones fueron confirmadas por el responsable de la documentación durante la revisión del borrador el 19/11/2026. Los cambios en los requisitos quedan registrados en [DEC-001 y DEC-002](../decisiones/registro-decisiones.md#decisiones) y se incorporan a la especificación mediante [SC-001 y SC-002](../cambios/registro-solicitudes-cambio.md#solicitudes). Las concreciones de análisis se circunscriben a esta descripción.

| Asunto | Acuerdo confirmado | Requisito canónico |
| --- | --- | --- |
| Personas y cuentas | Una única cuenta personal de Simbiosis por persona registrada, sin cuentas compartidas. Las modalidades de acceso pertenecen a esa misma cuenta. | FR-218; se conserva la vinculación de accesos de FR-190. |
| Compatibilidad de perfiles | Los perfiles de paciente, cuidador, nutricionista y coordinador pueden coexistir. Cada uno conserva sus condiciones de habilitación. | FR-212 actualizado. |
| Alcance de los perfiles | Esta descripción comprende únicamente a usuarios con al menos uno de los cuatro perfiles indicados. En el modelo de dominio, Usuario se representa como clase abstracta. | Concreción del alcance del análisis; FR-191 conserva su redacción. |
| Participación del paciente en el cuidado | Un paciente puede no tener cuidador o tener como máximo uno con relación de cuidado activa. Un cuidador puede cuidar a varios pacientes. | FR-219; se conservan FR-193 y FR-194. |
| Preferencias dietéticas | Solo los pacientes pueden seleccionar preferencias dietéticas. | FR-019 y FR-104 actualizados; nuevo FR-220. |
| Dirección y auditoría | Una dirección opcional puede compartirse; se detallan sus componentes. Cada actuación pertenece exclusivamente a un historial y se elimina con él. | Concreción de análisis aprobada para la descripción; FR-185 y FR-211 conservan su alcance. |
| Auditoría y eliminación | En esta descripción, las actuaciones permanecen en el historial cuando se elimina la cuenta afectada y no conservan una copia de su alias. No se contempla la eliminación de cuentas de coordinador. | Concreción para el análisis de FR-185; los plazos y condiciones de conservación siguen aplazados. |

Para acotar esta versión, se aplaza el desarrollo de los siguientes aspectos. Este aplazamiento no elimina requisitos ni establece políticas nuevas sobre conservación o acceso.

| Aspecto | Tratamiento en esta versión |
| --- | --- |
| Relaciones de cuidado | Se describen las relaciones vigentes. El registro de solicitudes pendientes, relaciones finalizadas y sucesivas relaciones entre las mismas personas queda aplazado. |
| Acreditación profesional | Se consideran la documentación aportada y su aprobación. Los tipos concretos de documentos admisibles, las nuevas aportaciones y el historial de revisiones quedan aplazados. |
| Aprobaciones y auditoría | Se conserva el historial elemental exigido por FR-185. No se desarrollan expedientes adicionales de aprobación ni historiales separados de revisión documental. |
| Condiciones de uso de la cuenta | La descripción conserva el estado y, cuando procede, la duración del bloqueo. Las condiciones de activación, suspensión, inactividad, expulsión y eliminación, incluidos sus plazos, siguen en el catálogo y las actas de origen. |
| Eliminación y conservación | FR-211 mantiene la conservación del contenido publicado tras eliminar la cuenta de un cuidador. Para la auditoría se aplica la concreción indicada arriba; los plazos y condiciones de conservación y la identificación de la autoría del contenido publicado quedan aplazados. |

### 9.2 Gestión de recetas

Durante la revisión documental del 19/11/2026 se confirmó que, para esta descripción, cada receta tiene un único autor y al menos un ingrediente; un ingrediente puede aparecer en varias recetas y, en cada una, se indica su cantidad y unidad. Cada receta validada tiene un único nutricionista validador, que puede ser su autor.

Para simplificar esta vista se excluye la eliminación de cuentas de cuidadores y nutricionistas, incluso si reúnen otros perfiles. FR-211 mantiene la conservación del contenido publicado por un cuidador tras eliminar su cuenta; el tratamiento de la autoría en ese caso queda fuera de esta vista. Esta delimitación no modifica los requisitos del producto.

Se confirmó también que un usuario puede crear ninguna, una o varias recetas, que un nutricionista puede validar ninguna, una o varias, y que un ingrediente puede no aparecer en ninguna receta o aparecer en varias, como máximo una vez en cada una.

Una receta puede no tener imágenes ni vídeos o incluir varios de cada tipo. Al ampliar el modelo con publicaciones de salud, cada imagen y cada vídeo se asocian a un único contenido: una receta o una publicación de salud.

Se confirmó que cada comentario y cada valoración corresponden a una única receta y tienen un único autor en esta vista; una receta puede tener ningún comentario o valoración, o varios. Cada respuesta corresponde al crearse a un único comentario de la misma receta.

Para simplificar esta vista, un comentario puede recibir ninguna, una o varias respuestas. Al eliminarse, sus respuestas se conservan sin asociación al comentario eliminado; al eliminarse una receta, se eliminan sus comentarios y valoraciones. Esta concreción no modifica la redacción canónica de los requisitos.

Queda pendiente precisar las multiplicidades no indicadas en esta descripción y el efecto de cambios posteriores en una receta validada. El historial de ediciones, las categorías y etiquetas, las marcas de utilidad de comentarios, las estadísticas y la calculadora nutricional se aplazan para esta vista; sus requisitos siguen vigentes.

### 9.3 Gestión de publicaciones de salud

Durante la revisión documental del 19/11/2026 se confirmó que cada publicación tiene un único nutricionista autor, título y texto; que un nutricionista puede crear ninguna, una o varias publicaciones; y que cada comentario tiene texto, fecha, hora, un único autor y una única publicación, con ninguna o varias publicaciones o comentarios por usuario y ningún o varios comentarios por publicación.

Se confirmó también que cada publicación puede tener ninguna o varias categorías, etiquetas, referencias y recursos; una categoría, etiqueta o referencia puede asociarse a ninguna o varias publicaciones. Cada documento PDF o recurso de audio pertenece a una única publicación. Las clases `Imagen` y `Video` se reutilizan entre recetas y publicaciones de salud: cada imagen o vídeo se asocia a un único contenido, sin compartirse entre ellos.

La revisión y aprobación por el coordinador corresponden a los requisitos de moderación y se estudiarán en ese módulo. La extensión máxima y las normas editoriales siguen pendientes en el acta general. Los casos en los que la eliminación de una cuenta deje contenido sin autor asociado quedan fuera de esta vista; los requisitos de conservación permanecen vigentes. El detalle de los «me gusta» y el tratamiento de comentarios y recursos cuando se elimina una publicación quedan pendientes de aclaración.

### 9.4 Moderación de contenidos

Se confirmó que cada reporte tiene un único autor, una categoría y un único contenido; que varios reportes pueden afectar al mismo contenido; y que cada reporte está pendiente o lo resuelve un único coordinador. Para el modelo se acordó agrupar los tipos reportables bajo un concepto común de contenido.

Para simplificar esta vista se excluye el reporte de perfiles de usuario. UR-09 y FR-120 mantienen su alcance; la representación de estos reportes queda aplazada.

Se confirmó que las expresiones prohibidas se eliminan con la lista que las contiene.

Como propuesta para esta vista, cada actuación afecta a un único contenido, tiene un único coordinador y puede relacionarse con un reporte; un reporte puede tener varias actuaciones. Una apelación corresponde a una actuación de eliminación y tiene un único usuario autor; una eliminación puede recibir ninguna o varias apelaciones. Las multiplicidades de las listas y expresiones de §7.3 también son propuestas. Estas concreciones son provisionales y no modifican los requisitos.

Los detalles del contenido del foro no descritos en el apartado 4, las reglas y sanciones, el contenido y la resolución de las apelaciones, las notificaciones, los intentos bloqueados, los criterios de prioridad y las estadísticas se dejan abiertos. También queda por precisar la conservación de reportes, contenidos y actuaciones cuando se elimina una cuenta o un contenido. FR-149 está retirado, aunque FR-152 menciona moderadores; esta vista representa al coordinador y no resuelve la discrepancia del catálogo.

### 9.5 Foro

Durante la revisión documental del 21/11/2026 se acordó, para esta descripción, tratar el hilo como publicación inicial y las respuestas como comentarios del mismo hilo. Se confirmaron la autoría única de hilos y comentarios, la pertenencia de cada comentario a un único hilo, la posibilidad de responder a cualquier profundidad y la participación de coordinadores. También se acordó que los hilos y comentarios pueden recibir «me gusta», con un máximo de uno por usuario y contenido y posibilidad de retirarlo.

Se acordó que, al eliminar un hilo, se eliminan todos sus comentarios, incluidas las respuestas. Esta concreción permite representar los comentarios como partes del hilo en la vista del dominio. La conservación de reportes y actuaciones permanece pendiente de aclaración en el apartado 9.4. La restauración de hilos eliminados por moderación y el tratamiento de sus comentarios quedan pendientes de consulta con el cliente en otra iteración, sin modificar FR-139.

Para simplificar la vista se propone que, al eliminar un comentario, permanezca un elemento que indique que fue eliminado y permita conservar las referencias de sus respuestas, sin mostrar su contenido ni su autor. Debe aclararse su compatibilidad con la eliminación permanente prevista en FR-028 antes de considerarlo resuelto. Esta propuesta no cambia el requisito.

Las etiquetas y las reglas detalladas de archivo quedan pendientes de consulta. La búsqueda por nombre de autor y alias no se modela en esta vista. Las menciones se limitan a comentarios; su modelado y el de las notificaciones se aplazan. También se aplazan los mensajes directos y el seguimiento entre usuarios. El seguimiento de hilos sí se incluye. La distinción entre «publicaciones» y «comentarios» en FR-030 y FR-033 debe contrastarse con la interpretación del hilo como publicación inicial; los requisitos mantienen su redacción y alcance.

### 9.6 Gestión de datos de salud

Durante la revisión documental del 21/11/2026 se acordó que cada paciente tenga un único historial, aunque pueda estar vacío, y que cada historial pertenezca a un único paciente. Las mediciones fisiológicas, los resultados de laboratorio y las notas pertenecen a un único historial y se eliminan con él. Para esta vista se distingue la presión arterial mediante sus valores sistólico y diastólico.

Se acordó también que cada alerta crítica corresponde a una única medición. La representación de alertas y umbrales, recordatorios y autorizaciones se aplaza para iteraciones posteriores, con las aclaraciones necesarias al cliente; los requisitos correspondientes siguen vigentes. También quedan para una iteración posterior la estructura y el uso de parámetros de laboratorio, incluida su posible compartición entre pacientes, y la unidad de la altura. La fecha asociada a la nota es una concreción de esta vista. No se establecen aquí políticas adicionales de conservación ni de eliminación de cuentas.

### 9.7 Guía interactiva

Durante la revisión documental del 21/11/2026 se acordó, para esta descripción, considerar una única guía con temas y pasos, tutoriales asociados cada uno a un único tema y un único punto de reanudación por usuario. Estas concreciones acotan el análisis y no modifican los requisitos.

Se acordó que los temas puedan conservarse al eliminar una guía, y que los pasos y tutoriales se eliminen con su tema. La fecha de última actualización del punto de reanudación es una concreción de esta vista. El tratamiento del punto de reanudación cuando se elimina el tema que contiene su paso queda pendiente de aclaración.

Se aplazan para una iteración posterior y su aclaración con el cliente el tratamiento del progreso de visitantes sin cuenta, la vinculación de los temas con las secciones de la plataforma y la organización de la búsqueda por palabras clave. El recorrido de bienvenida se deja fuera de esta vista; FR-207 mantiene su alcance y su independencia de la ayuda contextual. Las ayudas visuales se consideran elementos de interfaz y no se desarrollan como conceptos separados en esta descripción. La posible reutilización de `Video` se revisará con las restricciones de asociación de recetas y publicaciones de salud. Los requisitos de acceso, ayuda contextual, búsqueda y progreso siguen vigentes.

## 10 Fuentes y trazabilidad

### 10.1 Gestión de usuarios

El [catálogo de requisitos](../requisitos/catalogo-requisitos.md) conserva la redacción canónica de UR, FR y NFR. Las aclaraciones de requisitos de esta revisión se han incorporado al catálogo, conservando los identificadores existentes y asignando identificadores nuevos a los requisitos nuevos.

| Apartado | Fuentes de la información |
| --- | --- |
| 1. Alcance | [Visión y alcance](../vision/vision_y_alcance.md), §2.2; [SRS](../requisitos/srs.md), §§9 y 10.3. |
| 2.1. Identidad y cuenta | [Acta general](acta-captura-requisitos-generales.md), §1.1; [acta de UR-01](acta-captura-requisitos-ur-01.md), §§2.1, 2.2 y 2.4; [acta de UC-05](acta-acuerdos-uc-05-actualizar-perfil.md), §2; acuerdos del apartado 9.1 de esta acta. Catálogo: FR-002, FR-004, FR-009, FR-188, FR-192 y FR-218. |
| 2.2. Perfiles | [Acta general](acta-captura-requisitos-generales.md), §§1.2 y 1.3; [acta técnica y operativa](acta-acuerdos-tecnicos-operativos.md), §2.3.2; acuerdos del apartado 9.1 de esta acta. Catálogo: FR-181 y FR-212. |
| 2.3. Relaciones de cuidado | [Acta general](acta-captura-requisitos-generales.md), §§1.2 y 2; acuerdos del apartado 9.1 de esta acta. Catálogo: FR-193, FR-194 y FR-219. |
| 2.4. Acreditación profesional | [Acta de UR-01](acta-captura-requisitos-ur-01.md), §2.6; [acta técnica y operativa](acta-acuerdos-tecnicos-operativos.md), §2.3.2. Catálogo: FR-014, FR-181 y FR-191. |
| 2.5. Administración | Catálogo: FR-181–FR-186; concreción de auditoría del apartado 9.1 de esta acta. |
| 9.1. Límites de la descripción | [Acta general](acta-captura-requisitos-generales.md), §2; [acta técnica y operativa](acta-acuerdos-tecnicos-operativos.md), §2.2.4. Catálogo: FR-208–FR-211. |

Los acuerdos del apartado 9.1 son la fuente de FR-218, de la ampliación de FR-212 y de FR-219, incorporados mediante SC-001, y de la restricción de preferencias dietéticas incorporada mediante SC-002. Los aspectos aplazados conservan su estado pendiente; las decisiones posteriores se incorporarán con su procedencia y estado de validación.

### 10.2 Gestión de recetas

| Información | Fuentes |
| --- | --- |
| Alcance y funciones | [Visión y alcance](../vision/vision_y_alcance.md), §2.2; [acta general](acta-captura-requisitos-generales.md), §3. |
| Datos e ingredientes | [Catálogo de requisitos](../requisitos/catalogo-requisitos.md), FR-056–FR-058 y FR-086; [acta de UC-21](acta-acuerdos-uc-21-buscar-recetas.md), §2; aclaración de cantidad y unidad del apartado 9.2. |
| Autoría y validación | [Acta general](acta-captura-requisitos-generales.md), §§2 y 3; catálogo, FR-054, FR-055, FR-066, FR-204, FR-205 y FR-211; límites de la vista del apartado 9.2. |
| Comentarios y valoraciones | [Acta general](acta-captura-requisitos-generales.md), §§2–4; catálogo, FR-153, FR-156, FR-159, FR-161, FR-162, FR-169 y FR-211; concreciones del apartado 9.2. |
| Alcance y cuestiones aplazadas | [Modelo de casos de uso](../modelos/modelo-casos-de-uso.md), §§1 y 4.2; catálogo, FR-059–FR-065 y FR-085–FR-119. |

### 10.3 Gestión de publicaciones de salud

| Información | Fuentes |
| --- | --- |
| Publicaciones y autoría | [Acta general](acta-captura-requisitos-generales.md), §5; [SRS](../requisitos/srs.md), glosario; [catálogo](../requisitos/catalogo-requisitos.md), UR-07 y FR-067–FR-069, FR-075–FR-076, FR-079 y FR-083. |
| Clasificación y recursos | Catálogo, FR-070–FR-074 y FR-081; aclaraciones del apartado 9.3. |
| Participación | Acta general, §5; catálogo, FR-080; aclaraciones sobre comentarios del apartado 9.3. |
| Moderación | Catálogo, FR-134 y FR-135; apartado 7 de esta acta. |

### 10.4 Moderación de contenidos

| Información | Fuentes |
| --- | --- |
| Reportes y resolución | [Acta general](acta-captura-requisitos-generales.md), §4; [catálogo](../requisitos/catalogo-requisitos.md), UR-09, FR-120 y FR-122–FR-126; aclaraciones del apartado 9.4. |
| Actuaciones y apelaciones | [Acta de acuerdos técnicos y operativos](acta-acuerdos-tecnicos-operativos.md), §2.4.1; catálogo, UR-10, FR-132–FR-139, FR-142 y FR-146; propuestas del apartado 9.4. |
| Expresiones prohibidas | Catálogo, FR-127–FR-130 y FR-150; propuesta del apartado 9.4. |

### 10.5 Foro

| Información | Fuentes |
| --- | --- |
| Participación e identidad | [Acta general](acta-captura-requisitos-generales.md), §§1.1 y 4; [acta de UR-01](acta-captura-requisitos-ur-01.md), §2.1; [catálogo](../requisitos/catalogo-requisitos.md), FR-021, FR-192, FR-195 y FR-206; acuerdos del apartado 9.5. |
| Hilos y comentarios | Catálogo, UR-04, FR-022–FR-028 y FR-032; acuerdos y propuesta del apartado 9.5. |
| Seguimiento y «me gusta» | Catálogo, FR-029–FR-031 y FR-039; acuerdos del apartado 9.5. |
| Moderación y aspectos aplazados | Acta general, §4; catálogo, FR-033–FR-040, FR-120, FR-127–FR-130, FR-196 y FR-197; apartados 7 y 9.5 de esta acta. |

### 10.6 Gestión de datos de salud

| Información | Fuentes |
| --- | --- |
| Historial y mediciones | [Acta de UR-05](acta-captura-requisitos-ur-05.md), §§2.1 y 2.5; [catálogo](../requisitos/catalogo-requisitos.md), UR-05, FR-041, FR-049, FR-050 y FR-216; acuerdos del apartado 9.6. |
| Laboratorio y notas | Acta de UR-05, §2.2; catálogo, FR-042 y FR-053; concreciones del apartado 9.6. |
| Alertas y aspectos aplazados | Acta de UR-05, §§2.4, 2.6 y 2.7; catálogo, FR-043–FR-046, FR-051–FR-052 y FR-198–FR-203; acuerdo y límites del apartado 9.6. |

### 10.7 Guía interactiva

| Información | Fuentes |
| --- | --- |
| Temas, pasos y tutoriales | [Visión y alcance](../vision/vision_y_alcance.md), §2.2; [catálogo](../requisitos/catalogo-requisitos.md), UR-12, FR-173, FR-175 y FR-179; acuerdos del apartado 9.7. |
| Progreso y aspectos aplazados | Catálogo, FR-172, FR-174, FR-176–FR-178, FR-180 y FR-207; [acta general](acta-captura-requisitos-generales.md), §6; acuerdos y límites del apartado 9.7. |

## 11 Revisión y continuidad

Esta versión incorpora las aclaraciones sobre identidad, perfiles, cuidado, recetas, foro, datos de salud, publicaciones de salud, moderación de contenidos y guía interactiva. Su alcance sigue siendo parcial: los aspectos aplazados del apartado 9 no se consideran resueltos.

Las futuras ampliaciones del acta podrán incorporar otros módulos del Documento de Visión y Alcance. Los resultados del análisis conceptual se mantendrán en el modelo de dominio, con referencia a los apartados que los respalden.

## 12 Historial de versiones

| Versión | Fecha | Cambio |
| --- | --- | --- |
| 1.0 | 24/11/2026 | Se cierra el acta con su alcance acotado, manteniendo las propuestas provisionales y las cuestiones pendientes de aclaración. |
| 0.21 | 21/11/2026 | Se concretan las relaciones, la eliminación y el punto de reanudación de la guía interactiva. |
| 0.20 | 21/11/2026 | Se incorpora una descripción inicial de la guía interactiva, con sus acuerdos y aspectos aplazados. |
| 0.19 | 21/11/2026 | Se incorpora una primera descripción del historial y los registros de salud, con acuerdos y cuestiones aplazadas. |
| 0.18 | 21/11/2026 | Se acuerda la eliminación de los comentarios y respuestas al eliminar un hilo. |
| 0.17 | 21/11/2026 | Se incorpora una descripción inicial del foro, con acuerdos, fuentes y aspectos pendientes de aclaración. |
| 0.16 | 19/11/2026 | Se incorpora una primera descripción de Moderación de contenidos, sus fuentes, acuerdos y propuestas pendientes. |
| 0.15 | 19/11/2026 | Se incorpora una descripción inicial de Gestión de publicaciones de salud y se identifican sus fuentes y aclaraciones pendientes. |
| 0.14 | 19/11/2026 | Se excluye de la vista de recetas la eliminación de cuentas de cuidadores y se precisa la autoría de recetas, comentarios y valoraciones. |
| 0.13 | 19/11/2026 | Se concretan las respuestas y la eliminación de comentarios y valoraciones en la vista de recetas. |
| 0.12 | 19/11/2026 | Se incorpora información sobre comentarios y valoraciones de recetas y su conservación tras eliminar la cuenta de un cuidador. |
| 0.11 | 19/11/2026 | Se concretan las asociaciones de imágenes y vídeos con recetas para la primera vista del módulo. |
| 0.10 | 19/11/2026 | Se precisan las multiplicidades de autoría, validación e ingredientes y se limita a una la aparición de cada ingrediente en una receta. |
| 0.9 | 19/11/2026 | Se excluye de la vista de Gestión de recetas la eliminación de cuentas de nutricionistas, incluso cuando reúnen otros perfiles. |
| 0.8 | 19/11/2026 | Se agrupa la información por módulos y se añaden apartados pendientes para los restantes; los acuerdos y las fuentes se reúnen al final. |
| 0.7 | 19/11/2026 | Se añade una primera descripción de Gestión de recetas y se registran las aclaraciones sobre cantidad y unidad de los ingredientes y conservación de recetas al eliminar una cuenta de cuidador. |
| 0.6 | 19/11/2026 | Se acota la descripción a los cuatro perfiles elegidos y se cierra la cuestión sobre la representación de Usuario en el modelo de dominio. |
| 0.5 | 19/11/2026 | Se depura la información para el análisis conceptual y se precisa la conservación de actuaciones sin copia del alias tras eliminar una cuenta. Se deja abierta la representación de usuarios sin perfil habilitado. |
| 0.4 | 19/11/2026 | Preferencias dietéticas exclusivas de pacientes y concreción de direcciones compartidas, documentación e historial de auditoría conforme al análisis estructural. SC-002 registra el cambio en requisitos; queda abierta la conservación de actuaciones tras eliminar cuentas. |
| 0.3 | 19/11/2026 | Se depura la descripción para conservar la información relevante para el análisis de clases, datos y relaciones. Se retiran del apartado 2 los flujos de uso, las referencias a otros módulos y los detalles técnicos o temporales que no afectan a la estructura descrita. Se conservan los acuerdos confirmados y su trazabilidad. |
| 0.2 | 19/11/2026 | Se incorporan las decisiones confirmadas: cuenta personal única, compatibilidad de perfiles y máximo de un cuidador activo por paciente. Se acotan los restantes aspectos y se registra su reflejo en la especificación mediante SC-001. |
| 0.1 | 19/11/2026 | Borrador inicial centrado en Gestión de usuarios. Síntesis de información existente y preguntas para completar su descripción conceptual. |
