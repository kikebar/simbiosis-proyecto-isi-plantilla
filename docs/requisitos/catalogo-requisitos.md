# Proyecto Simbiosis

## Catálogo de requisitos

**Versión:** 1.16
**Fecha:** 19/11/2026
**Estado:** UR, FR y NFR de la primera versión consolidados
**Fuente de verdad:** este catálogo contiene el texto canónico de los requisitos de usuario (UR), funcionales (FR) y no funcionales (NFR).

Este documento complementa la [Especificación de requisitos de software](./srs.md). La SRS organiza el contexto, el alcance, las decisiones pendientes y los modelos; este catálogo conserva una única copia de cada requisito y sus relaciones.

La referencia común al catálogo canónico y a la SRS aparece en la cabecera. La procedencia de cada incorporación o modificación queda registrada en el control de cambios.

## Índice

1. [Convenciones](#1-convenciones)
2. [Objetivos de negocio relacionados](#2-objetivos-de-negocio-relacionados)
3. [Requisitos de usuario](#3-requisitos-de-usuario)
4. [Requisitos funcionales](#4-requisitos-funcionales)
5. [Requisitos no funcionales](#5-requisitos-no-funcionales)
6. [Matriz de trazabilidad](#6-matriz-de-trazabilidad)
7. [Control de cambios](#7-control-de-cambios)

## 1. Convenciones

- `BO-0X`: objetivo de negocio, cuando se necesite conservar la relación con el Documento de Visión y Alcance.
- `UR-0X`: requisito de usuario.
- `FR-0XX`: requisito funcional.
- `NFR-0XX`: requisito no funcional.
- `UC-0X`: caso de uso relacionado, cuando exista un modelo que lo interprete.

Los UR se redactan desde la perspectiva de la persona usuaria: «El [tipo de usuario] podrá [acción] [finalidad]». Cada UR expresa una única necesidad de alto nivel.

Los FR se redactan con el patrón «El sistema debe [verbo] [objeto] [condición]». Cada FR expresa una única responsabilidad del sistema y es verificable.

Cada NFR expresa una única condición de calidad o restricción medible y verificable, con su ámbito global o ligado a un UR o FR concreto.

## 2. Objetivos de negocio relacionados

| ID | Objetivo de negocio | UR relacionados |
| --- | --- | --- |
| BO-01 | La organización busca mejorar la calidad de vida de los pacientes con Enfermedades Inflamatorias Intestinales (EII) mediante el acceso a recetas adaptadas a sus necesidades de salud. | UR-05, UR-06, UR-08 |
| BO-02 | La organización pretende ofrecer a los pacientes con EII una herramienta que les permita gestionar mejor su dieta para controlar los síntomas de la enfermedad. | UR-05, UR-08 |
| BO-03 | La organización busca asegurar la calidad clínica de las recetas compartidas en la aplicación. | UR-06, UR-07, UR-10, UR-13 |
| BO-04 | La organización busca fomentar la colaboración entre pacientes, cuidadores y profesionales de la salud, creando una comunidad activa que comparta conocimiento y experiencias. | UR-04, UR-06, UR-07, UR-11 |
| BO-05 | La organización quiere fomentar una comunidad activa y de apoyo mutuo para pacientes con EII. | UR-04, UR-06, UR-07, UR-11 |
| BO-06 | La organización debe asegurar un entorno seguro y confiable para la comunidad EII. | UR-04, UR-09, UR-10, UR-13 |

## 3. Requisitos de usuario

| ID | Requisito de usuario | BO relacionados | FR asociados | Estado |
| --- | --- | --- | --- | --- |
| UR-01 | El usuario podrá registrarse en la plataforma proporcionando información básica como nombre, correo electrónico y contraseña, para acceder a las funcionalidades. | — | FR-001, FR-002, FR-003, FR-004, FR-005, FR-006, FR-007, FR-008, FR-009, FR-010, FR-011, FR-012, FR-013, FR-014, FR-188, FR-189, FR-190, FR-191, FR-192, FR-193, FR-194, FR-213, FR-214, FR-215, FR-218, FR-219 | Vigente |
| UR-02 | El usuario podrá autenticarse en la plataforma introduciendo sus credenciales de acceso. | — | FR-015, FR-016, FR-017, FR-018 | Vigente |
| UR-03 | El usuario podrá gestionar su perfil en la plataforma, actualizando datos personales y de contacto cuando lo requiera. | — | FR-019, FR-020, FR-220 | Vigente |
| UR-04 | El usuario registrado podrá participar en un foro colaborativo, creando nuevos hilos de discusión, respondiendo a publicaciones existentes y compartiendo opiniones o sugerencias. | BO-04, BO-05, BO-06 | FR-021, FR-022, FR-023, FR-024, FR-025, FR-026, FR-027, FR-028, FR-029, FR-030, FR-031, FR-032, FR-033, FR-034, FR-035, FR-036, FR-037, FR-038, FR-039, FR-040, FR-195, FR-196, FR-197 | Vigente |
| UR-05 | El paciente podrá introducir y gestionar sus datos fisiológicos y de salud, accediendo a un historial detallado y actualizando la información según sea necesario. | BO-01, BO-02 | FR-041, FR-042, FR-043, FR-044, FR-045, FR-046, FR-047, FR-048, FR-049, FR-050, FR-051, FR-052, FR-053, FR-198, FR-199, FR-200, FR-201, FR-202, FR-203, FR-216, FR-217 | Vigente |
| UR-06 | El usuario registrado podrá crear recetas en la plataforma, incluyendo detalles como ingredientes, instrucciones de preparación, tiempo de cocción, porciones, e incorporando imágenes o videos, para compartirlas con la comunidad. | BO-01, BO-03, BO-04, BO-05 | FR-054, FR-055, FR-056, FR-057, FR-058, FR-059, FR-060, FR-061, FR-062, FR-063, FR-064, FR-065, FR-066, FR-204, FR-205 | Vigente |
| UR-07 | El nutricionista podrá crear y publicar consejos de vida saludable en la plataforma, incluyendo texto formateado, imágenes, videos y enlaces a fuentes confiables, para ofrecer información relevante sobre nutrición, ejercicio y bienestar general. | BO-03, BO-04, BO-05 | FR-067, FR-068, FR-069, FR-070, FR-071, FR-072, FR-073, FR-074, FR-075, FR-076, FR-077, FR-078, FR-079, FR-080, FR-081, FR-082, FR-083, FR-084, FR-206 | Vigente |
| UR-08 | El usuario podrá buscar recetas en la plataforma utilizando palabras clave, filtros avanzados (ingredientes, tiempo de preparación, nivel de dificultad) y categorías específicas (tipo de comida o restricciones dietéticas). | BO-01, BO-02 | FR-085, FR-086, FR-087, FR-088, FR-089, FR-090, FR-091, FR-092, FR-093, FR-094, FR-095, FR-096, FR-097, FR-098, FR-099, FR-100, FR-101, FR-102, FR-103, FR-104, FR-105, FR-106, FR-107, FR-108, FR-109, FR-110, FR-111, FR-112, FR-113, FR-114, FR-115, FR-116, FR-117, FR-118, FR-119 | Vigente |
| UR-09 | El usuario registrado podrá reportar contenido inapropiado, como recetas, comentarios, publicaciones o perfiles de usuario, seleccionando una categoría de reporte (por ejemplo, spam o contenido ofensivo) y añadiendo comentarios adicionales si lo considera necesario. | BO-06 | FR-120, FR-121, FR-122, FR-123, FR-124, FR-125, FR-126 | Vigente |
| UR-10 | El coordinador podrá moderar el contenido reportado o inadecuado, aplicando reglas de uso y garantizando un entorno seguro en la plataforma. | BO-03, BO-06 | FR-127, FR-128, FR-129, FR-130, FR-131, FR-132, FR-133, FR-134, FR-135, FR-136, FR-137, FR-138, FR-139, FR-142, FR-145, FR-146, FR-147, FR-148, FR-149, FR-150, FR-151, FR-152 | Vigente |
| UR-11 | El usuario registrado podrá valorar las recetas y dejar comentarios para compartir opiniones, sugerencias o preguntas sobre las recetas publicadas. | BO-04, BO-05 | FR-153, FR-154, FR-155, FR-156, FR-157, FR-158, FR-159, FR-160, FR-161, FR-162, FR-163, FR-164, FR-165, FR-166, FR-167, FR-168, FR-169, FR-170, FR-171 | Vigente |
| UR-12 | El usuario podrá acceder a una guía interactiva con instrucciones paso a paso sobre las funcionalidades de la plataforma, incluyendo registro, búsqueda, publicación de recetas y uso del foro, con elementos visuales y tutoriales multimedia. | — | FR-172, FR-173, FR-174, FR-175, FR-176, FR-177, FR-178, FR-179, FR-180, FR-207 | Vigente |
| UR-13 | El coordinador podrá gestionar las cuentas de usuario desde un panel de administración, incluyendo la aprobación de nuevas cuentas, la suspensión de cuentas activas y la eliminación de cuentas cuando sea necesario. | BO-03, BO-06 | FR-181, FR-182, FR-183, FR-184, FR-185, FR-186, FR-187, FR-208, FR-209, FR-210, FR-211, FR-212, FR-219 | Vigente |

## 4. Requisitos funcionales

| ID | Requisito funcional | UR asociados | UC relacionados | Estado |
| --- | --- | --- | --- | --- |
| FR-001 | El sistema debe permitir a cualquier usuario completar el formulario de registro, creando con ello una cuenta en estado pendiente de activación. | UR-01 | — | Vigente |
| FR-002 | El sistema debe requerir, durante el registro, nombre completo, dirección de correo electrónico válida, número de teléfono y contraseña. | UR-01 | — | Vigente |
| FR-003 | El sistema debe enviar un correo electrónico de verificación a la dirección de correo proporcionada para confirmar el registro. | UR-01 | — | Vigente |
| FR-004 | El sistema debe verificar que la dirección de correo electrónico no esté registrada previamente antes de completar el registro. | UR-01 | — | Vigente |
| FR-005 | El sistema debe mostrar en el formulario de registro dos casillas de verificación independientes: una para la aceptación de los términos y condiciones y otra para la aceptación de la política de privacidad. | UR-01 | — | Vigente |
| FR-006 | El sistema debe permitir el registro mediante cuenta de Google como opción de autenticación externa. | UR-01 | — | Vigente |
| FR-007 | El sistema debe mostrar mensajes de error específicos en el formulario de registro indicando la causa (por ejemplo, campo vacío o formato de correo incorrecto). | UR-01 | — | Vigente |
| FR-008 | El sistema debe implementar un CAPTCHA con alternativa accesible en audio en el formulario de registro, sin ofrecer una vía de omisión, para prevenir registros automatizados. | UR-01 | — | Vigente |
| FR-009 | El sistema debe registrar, en UTC, la fecha y hora en que el usuario verifica su correo electrónico durante el proceso de registro. | UR-01 | — | Vigente |
| FR-010 | El sistema debe mostrar una pantalla de confirmación cuando el registro se complete, es decir, cuando el usuario verifique su correo electrónico. | UR-01 | — | Vigente |
| FR-011 | El sistema debe validar en tiempo real la fortaleza de la contraseña, indicando mediante color y texto qué condición de la política de contraseñas falta por cumplir. | UR-01 | — | Vigente |
| FR-012 | El sistema debe validar en tiempo real el formato del correo electrónico al perder el foco del campo, según los estándares definidos. | UR-01 | — | Vigente |
| FR-013 | El sistema debe aplicar la siguiente política de contraseñas: mínimo 8 caracteres, al menos una mayúscula, una minúscula, un número y un carácter especial. | UR-01 | — | Vigente |
| FR-014 | El sistema debe requerir a quien se registre como nutricionista la carga de un archivo PDF con su documentación oficial de titulación y profesión, con un tamaño máximo de 10 MB. | UR-01 | — | Vigente |
| FR-015 | El sistema debe permitir el inicio de sesión mediante correo electrónico y contraseña válidos. | UR-02 | — | Vigente |
| FR-016 | El sistema debe permitir recuperar o restablecer la contraseña exclusivamente mediante un enlace enviado al correo electrónico asociado a la cuenta. | UR-02 | — | Vigente |
| FR-017 | Autenticación de dos factores. Requisito retirado; no se implementa en esta fase. | UR-02 | — | Retirado |
| FR-018 | El sistema debe permitir el inicio de sesión mediante cuenta de Google como opción de autenticación externa. | UR-02 | — | Vigente |
| FR-019 | El sistema debe permitir a los usuarios editar su información personal y las preferencias disponibles para su perfil en cualquier momento posterior al registro, con excepción del alias y del correo electrónico. | UR-03 | — | Vigente |
| FR-020 | El sistema debe permitir a los usuarios eliminar su cuenta mediante un proceso que incluya verificación de identidad con la contraseña actual. | UR-03 | — | Vigente |
| FR-021 | El sistema debe requerir que el usuario haya iniciado sesión para crear hilos, publicar comentarios, responder, seguir hilos y dar "me gusta" en el foro. | UR-04 | — | Vigente |
| FR-022 | El sistema debe permitir a los usuarios registrados crear hilos de discusión con título y cuerpo de contenido. | UR-04 | — | Vigente |
| FR-023 | El sistema debe permitir a los usuarios registrados publicar comentarios en los hilos de discusión con un límite de 1.000 caracteres por comentario. | UR-04 | — | Vigente |
| FR-024 | El sistema debe permitir responder a comentarios específicos dentro de un hilo, manteniendo la relación padre–hijo y visualizando la respuesta asociada al comentario original. | UR-04 | — | Vigente |
| FR-025 | El sistema debe enviar una notificación interna al autor de una publicación cuando reciba una respuesta, indicando el hilo y un enlace a la respuesta. | UR-04 | — | Vigente |
| FR-026 | El sistema debe enviar una notificación interna cuando se mencione a un usuario mediante "@alias", indicando el hilo y el comentario donde se realizó la mención. | UR-04 | — | Vigente |
| FR-027 | El sistema debe permitir a los usuarios editar sus propios comentarios durante los 15 minutos posteriores a su publicación. | UR-04 | — | Vigente |
| FR-028 | El sistema debe permitir a los usuarios eliminar permanentemente sus propios comentarios, de forma que dejen de ser visibles en el foro. | UR-04 | — | Vigente |
| FR-029 | El sistema debe permitir a los usuarios seguir hilos de discusión y listarlos en una sección de "Hilos seguidos" en su perfil. | UR-04 | — | Vigente |
| FR-030 | El sistema debe enviar notificaciones internas a los usuarios cuando haya nuevas publicaciones o comentarios en los hilos que siguen. | UR-04 | — | Vigente |
| FR-031 | El sistema debe permitir a los usuarios dar "me gusta" a publicaciones y mostrar el contador total de "me gusta" por publicación. | UR-04 | — | Vigente |
| FR-032 | El sistema debe mostrar la fecha y hora de cada publicación y comentario en formato **DD/MM/AAAA HH:mm (24 h)** junto al contenido. | UR-04 | — | Vigente |
| FR-033 | El sistema debe archivar automáticamente los hilos sin nuevas publicaciones ni comentarios durante 90 días, deshabilitando nuevos comentarios y manteniendo la visualización. | UR-04 | — | Vigente |
| FR-034 | El sistema debe permitir buscar publicaciones por nombre de autor con coincidencia exacta. | UR-04 | — | Vigente |
| FR-035 | El sistema debe permitir filtrar publicaciones por rango de fechas de publicación. | UR-04 | — | Vigente |
| FR-036 | El sistema debe permitir filtrar publicaciones por etiquetas asignadas a los hilos. | UR-04 | — | Vigente |
| FR-037 | El sistema debe permitir buscar por palabras clave en el título o el cuerpo de la publicación. | UR-04 | — | Vigente |
| FR-038 | El sistema debe permitir combinar los filtros de búsqueda anteriores en una misma consulta. | UR-04 | — | Vigente |
| FR-039 | El sistema debe mostrar una lista de publicaciones destacadas basada en el número de "me gusta" recibidos en las últimas 24 horas, ordenada de mayor a menor. | UR-04 | — | Vigente |
| FR-040 | El sistema debe mostrar una lista de publicaciones destacadas basada en el número de respuestas recibidas en las últimas 24 horas, ordenada de mayor a menor. | UR-04 | — | Vigente |
| FR-041 | El sistema debe permitir al paciente introducir manualmente sus datos fisiológicos (peso, altura, presión arterial, frecuencia cardíaca y temperatura corporal) mediante un formulario dedicado. | UR-05 | — | Vigente |
| FR-042 | El sistema debe permitir al paciente registrar resultados de análisis de laboratorio, incluyendo glucosa en sangre, colesterol y otros parámetros configurables, especificando siempre las unidades de medida correspondientes. | UR-05 | — | Vigente |
| FR-043 | El sistema debe enviar recordatorios internos al paciente para introducir sus datos fisiológicos con la frecuencia configurada en su perfil. | UR-05 | — | Vigente |
| FR-044 | El sistema debe permitir al paciente personalizar la frecuencia de los recordatorios (diaria, semanal, mensual). | UR-05 | — | Vigente |
| FR-045 | El sistema debe permitir al paciente autorizar a nutricionistas específicos para acceder a sus datos fisiológicos y de salud. | UR-05 | — | Vigente |
| FR-046 | El sistema debe validar la identidad de los nutricionistas autorizados mediante correo electrónico o identificación única antes de conceder acceso. | UR-05 | — | Vigente |
| FR-047 | El sistema debe permitir al paciente exportar sus datos fisiológicos y de salud en formato PDF. | UR-05 | — | Vigente |
| FR-048 | El sistema debe permitir al paciente exportar sus datos fisiológicos y de salud en formato CSV. | UR-05 | — | Vigente |
| FR-049 | El sistema debe mostrar el historial de datos fisiológicos introducidos por el paciente, ordenado por defecto de más reciente a más antiguo. | UR-05 | — | Vigente |
| FR-050 | El sistema debe representar los datos fisiológicos mediante gráficos visuales accesibles desde el perfil del paciente. | UR-05 | — | Vigente |
| FR-051 | El sistema debe generar alertas automáticas cuando los datos fisiológicos introducidos por el paciente superen los umbrales críticos definidos previamente por el nutricionista o por normas médicas generales configuradas en el sistema. | UR-05 | — | Vigente |
| FR-052 | El sistema debe registrar en el historial del paciente cada alerta crítica generada. | UR-05 | — | Vigente |
| FR-053 | El sistema debe permitir al paciente registrar síntomas o notas relacionadas con su estado de salud diario, con un límite de 500 caracteres por nota. | UR-05 | — | Vigente |
| FR-054 | El sistema debe permitir al usuario registrado crear nuevas recetas en la plataforma mediante un formulario dedicado. | UR-06 | — | Vigente |
| FR-055 | El sistema debe permitir al nutricionista publicar directamente como validadas las recetas que cree. | UR-06 | — | Vigente |
| FR-056 | El sistema debe proporcionar un formulario de publicación de recetas con campos obligatorios para: título de la receta, ingredientes, instrucciones de preparación, tiempo de cocción y número de porciones. | UR-06 | — | Vigente |
| FR-057 | El sistema debe permitir al usuario subir imágenes en formato JPEG o PNG como parte de la receta. | UR-06 | — | Vigente |
| FR-058 | El sistema debe permitir al usuario subir videos en formato MP4, con un tamaño máximo de 100 MB, como parte de la receta. | UR-06 | — | Vigente |
| FR-059 | El sistema debe permitir al usuario clasificar las recetas por categorías (tipo de comida, restricciones dietéticas, nivel de dificultad, tiempo de preparación). | UR-06 | — | Vigente |
| FR-060 | El sistema debe permitir al usuario asignar etiquetas (palabras clave) a las recetas para facilitar la búsqueda y filtrado. | UR-06 | — | Vigente |
| FR-061 | El sistema debe permitir al usuario editar sus recetas publicadas en cualquier momento y mantener un registro de las ediciones realizadas. | UR-06 | — | Vigente |
| FR-062 | El sistema debe permitir al usuario eliminar sus recetas publicadas, solicitando confirmación previa para evitar eliminaciones accidentales. | UR-06 | — | Vigente |
| FR-063 | El sistema debe mostrar al usuario el historial completo de sus recetas publicadas, incluyendo las ediciones realizadas y el número de visualizaciones de cada receta. | UR-06 | — | Vigente |
| FR-064 | El sistema debe mostrar estadísticas de cada receta publicada, incluyendo el número de visualizaciones, comentarios y calificaciones recibidas. | UR-06 | — | Vigente |
| FR-065 | El sistema debe ofrecer una calculadora nutricional automática que estime calorías, proteínas, carbohidratos y grasas por porción a partir de los ingredientes ingresados. | UR-06 | — | Vigente |
| FR-066 | El sistema debe mostrar una insignia distintiva en las recetas que hayan superado la validación de un nutricionista, con independencia de si su autor es un nutricionista, un paciente o un cuidador. | UR-06 | — | Vigente |
| FR-067 | El sistema debe permitir al nutricionista crear un consejo de vida saludable en la plataforma mediante un formulario dedicado. | UR-07 | — | Vigente |
| FR-068 | El sistema debe permitir al nutricionista publicar los consejos creados en la plataforma. | UR-07 | — | Vigente |
| FR-069 | El sistema debe proporcionar un editor de texto con opciones de formato (negrita, cursiva, listas numeradas y con viñetas) para redactar consejos de vida saludable. | UR-07 | — | Vigente |
| FR-070 | El sistema debe permitir al nutricionista adjuntar imágenes en formato JPEG o PNG a los consejos. | UR-07 | — | Vigente |
| FR-071 | El sistema debe permitir al nutricionista adjuntar videos en formato MP4 de hasta 100 MB a los consejos. | UR-07 | — | Vigente |
| FR-072 | El sistema debe permitir al nutricionista adjuntar recursos adicionales en formato PDF o audio a los consejos. | UR-07 | — | Vigente |
| FR-073 | El sistema debe permitir al nutricionista clasificar los consejos de vida saludable en categorías predefinidas (nutrición, ejercicio, salud mental, hábitos de sueño). | UR-07 | — | Vigente |
| FR-074 | El sistema debe permitir al nutricionista etiquetar los consejos con palabras clave para facilitar la búsqueda y filtrado. | UR-07 | — | Vigente |
| FR-075 | El sistema debe permitir al usuario (paciente o cuidador) acceder libremente a los consejos de vida saludable publicados. | UR-07 | — | Vigente |
| FR-076 | El sistema debe mostrar en cada consejo la información del autor: nombre completo, especialidad médica y una breve biografía profesional. | UR-07 | — | Vigente |
| FR-077 | El sistema debe permitir al nutricionista editar sus propios consejos después de publicarlos. | UR-07 | — | Vigente |
| FR-078 | El sistema debe permitir al nutricionista eliminar sus propios consejos después de publicarlos, solicitando confirmación previa. | UR-07 | — | Vigente |
| FR-079 | El sistema debe permitir al nutricionista programar la publicación de sus consejos indicando fecha y hora futuras. | UR-07 | — | Vigente |
| FR-080 | El sistema debe proporcionar al nutricionista estadísticas sobre la interacción de los usuarios con sus consejos, incluyendo número de visualizaciones, "me gusta" y comentarios recibidos. | UR-07 | — | Vigente |
| FR-081 | El sistema debe permitir al nutricionista incluir referencias o enlaces a estudios científicos o fuentes confiables dentro de sus consejos. | UR-07 | — | Vigente |
| FR-082 | El sistema debe permitir al nutricionista previsualizar sus consejos antes de publicarlos. | UR-07 | — | Vigente |
| FR-083 | El sistema debe asegurar que solo nutricionistas verificados puedan publicar consejos de vida saludable. | UR-07 | — | Vigente |
| FR-084 | El sistema debe incluir una página dedicada que muestre todos los consejos publicados, organizada por categorías y popularidad. | UR-07 | — | Vigente |
| FR-085 | El sistema debe permitir al usuario buscar recetas mediante palabras clave o frases en un campo de búsqueda dedicado. | UR-08 | — | Vigente |
| FR-086 | El sistema debe permitir buscar recetas por ingredientes seleccionados, mostrando solo las que los contengan. | UR-08 | — | Vigente |
| FR-087 | El sistema debe permitir excluir ingredientes de la búsqueda, como aquellos definidos como alérgenos o no deseados por el usuario. | UR-08 | — | Vigente |
| FR-088 | El sistema debe permitir buscar recetas por autor o creador específico. | UR-08 | — | Vigente |
| FR-089 | El sistema debe mostrar resultados de búsqueda con vista previa de cada receta, incluyendo título, imagen, calificación promedio y breve descripción. | UR-08 | — | Vigente |
| FR-090 | El sistema debe permitir filtrar recetas por tipo de comida (desayuno, almuerzo, cena) mediante selección múltiple. | UR-08 | — | Vigente |
| FR-091 | El sistema debe permitir filtrar recetas por tiempo de preparación (menos de 15 minutos, 30 minutos, más de una hora). | UR-08 | — | Vigente |
| FR-092 | El sistema debe permitir filtrar recetas por nivel de dificultad (fácil, intermedio, avanzado). | UR-08 | — | Vigente |
| FR-093 | El sistema debe permitir filtrar recetas por restricciones dietéticas (vegano, sin gluten, bajo en carbohidratos). | UR-08 | — | Vigente |
| FR-094 | El sistema debe permitir filtrar recetas por alergias e intolerancias alimentarias definidas en el perfil del usuario. | UR-08 | — | Vigente |
| FR-095 | El sistema debe permitir combinar múltiples criterios de búsqueda avanzada (ingredientes, tipo de comida, tiempo de preparación, restricciones dietéticas). | UR-08 | — | Vigente |
| FR-096 | El sistema debe permitir ordenar los resultados de búsqueda por relevancia respecto a los términos introducidos. | UR-08 | — | Vigente |
| FR-097 | El sistema debe permitir ordenar los resultados de búsqueda por popularidad (número de visualizaciones o "me gusta"). | UR-08 | — | Vigente |
| FR-098 | El sistema debe permitir ordenar los resultados de búsqueda por calificación promedio. | UR-08 | — | Vigente |
| FR-099 | El sistema debe permitir ordenar los resultados de búsqueda por fecha de publicación, mostrando primero las recetas más recientes. | UR-08 | — | Vigente |
| FR-100 | El sistema debe ofrecer sugerencias automáticas de búsqueda basadas en términos populares a medida que el usuario escribe. | UR-08 | — | Vigente |
| FR-101 | El sistema debe ofrecer sugerencias automáticas de búsqueda basadas en el historial personal del usuario. | UR-08 | — | Vigente |
| FR-102 | El sistema debe proporcionar alternativas relacionadas o correcciones ortográficas cuando una búsqueda no arroje resultados. | UR-08 | — | Vigente |
| FR-103 | El sistema debe permitir la búsqueda de recetas en múltiples idiomas, ajustando los resultados al idioma seleccionado por el usuario. | UR-08 | — | Vigente |
| FR-104 | El sistema debe recomendar recetas basadas en las preferencias alimenticias configuradas en el perfil del paciente. | UR-08 | — | Vigente |
| FR-105 | El sistema debe recomendar recetas basadas en el historial de búsqueda del usuario. | UR-08 | — | Vigente |
| FR-106 | El sistema debe recomendar recetas basadas en la información de salud del perfil del usuario (alergias, intolerancias). | UR-08 | — | Vigente |
| FR-107 | El sistema debe mostrar una sección de recetas similares en la vista detallada de cada receta, calculada en función de ingredientes y tipo de comida. | UR-08 | — | Vigente |
| FR-108 | El sistema debe mostrar una sección de recetas más populares basada en calificaciones y número de visualizaciones. | UR-08 | — | Vigente |
| FR-109 | El sistema debe enviar notificaciones internas al usuario cuando se publiquen nuevas recetas que coincidan con sus preferencias o historial de búsqueda. | UR-08 | — | Vigente |
| FR-110 | El sistema debe registrar el historial de búsquedas de cada usuario. | UR-08 | — | Vigente |
| FR-111 | El sistema debe permitir al usuario acceder a su historial de búsquedas desde su perfil. | UR-08 | — | Vigente |
| FR-112 | El sistema debe permitir al usuario guardar recetas como favoritas para acceder a ellas desde su perfil. | UR-08 | — | Vigente |
| FR-113 | El sistema debe permitir al usuario añadir recetas a listas personalizadas creadas en su perfil. | UR-08 | — | Vigente |
| FR-114 | El sistema debe permitir al usuario marcar recetas para leer más tarde en una lista separada de las favoritas. | UR-08 | — | Vigente |
| FR-115 | El sistema debe permitir al usuario descargar recetas en formato PDF para consulta sin conexión. | UR-08 | — | Vigente |
| FR-116 | El sistema debe permitir al usuario imprimir recetas en un formato optimizado para papel o PDF. | UR-08 | — | Vigente |
| FR-117 | El sistema debe permitir al usuario compartir recetas mediante enlaces directos para redes sociales o correo electrónico. | UR-08 | — | Vigente |
| FR-118 | El sistema debe mostrar estadísticas básicas de cada receta (número de visualizaciones, descargas y valoraciones). | UR-08 | — | Vigente |
| FR-119 | El sistema debe requerir que el usuario esté registrado e iniciado sesión para acceder a funciones de búsqueda avanzada y resultados personalizados. | UR-08 | — | Vigente |
| FR-120 | El sistema debe permitir al usuario registrado reportar recetas, publicaciones, comentarios y perfiles de usuario mediante una opción disponible junto al contenido. | UR-09 | — | Vigente |
| FR-121 | El sistema debe mostrar en cada receta, publicación, comentario y perfil de usuario un botón visible de "Reportar" accesible desde la interfaz principal. | UR-09 | — | Vigente |
| FR-122 | El sistema debe permitir al usuario seleccionar una categoría de reporte (spam, contenido ofensivo, información errónea, lenguaje inapropiado). | UR-09 | — | Vigente |
| FR-123 | El sistema debe permitir al usuario añadir un comentario opcional al reporte para proporcionar contexto adicional. | UR-09 | — | Vigente |
| FR-124 | El sistema debe registrar cada reporte en una base de datos centralizada con la siguiente información mínima: usuario que reporta, contenido reportado, categoría seleccionada, fecha y hora. | UR-09 | — | Vigente |
| FR-125 | El sistema debe notificar al usuario que ha realizado el reporte, confirmando que ha sido recibido y será revisado. | UR-09 | — | Vigente |
| FR-126 | El sistema debe notificar al usuario que reportó el contenido sobre la resolución final de su reporte, sin revelar datos personales del autor afectado. | UR-09 | — | Vigente |
| FR-127 | El sistema debe verificar automáticamente, antes de publicar, el contenido de hilos y comentarios contra una lista de palabras o frases prohibidas. | UR-10 | — | Vigente |
| FR-128 | El sistema debe mantener una lista editable por coordinadores de palabras o frases prohibidas. | UR-10 | — | Vigente |
| FR-129 | El sistema debe bloquear la publicación que contenga palabras o frases prohibidas y mostrar un mensaje de advertencia al usuario. | UR-10 | — | Vigente |
| FR-130 | El sistema debe permitir al usuario modificar el contenido bloqueado y volver a intentar su publicación. | UR-10 | — | Vigente |
| FR-131 | El sistema debe notificar a los coordinadores cuando un mismo usuario realice **3 intentos** de publicar contenido bloqueado dentro de **24 horas**. | UR-10 | — | Vigente |
| FR-132 | El sistema debe permitir al coordinador revisar y aprobar recetas antes de su publicación para verificar cumplimiento de políticas de la plataforma. | UR-10 | — | Vigente |
| FR-133 | El sistema debe permitir al coordinador editar o eliminar recetas y comentarios que no cumplan con las políticas de la plataforma, registrando las acciones realizadas. | UR-10 | — | Vigente |
| FR-134 | El sistema debe permitir al coordinador revisar y aprobar los consejos antes de su publicación para verificar cumplimiento de las políticas de la plataforma. | UR-10 | — | Vigente |
| FR-135 | El sistema debe permitir al coordinador editar o eliminar consejos o comentarios que incumplan las políticas de la plataforma, registrando las acciones realizadas. | UR-10 | — | Vigente |
| FR-136 | El sistema debe proporcionar a los coordinadores una herramienta de gestión de reportes que permita visualizar, filtrar y priorizar los reportes recibidos según tipo de infracción y fecha. | UR-10 | — | Vigente |
| FR-137 | El sistema debe permitir al coordinador eliminar, editar o mantener el contenido reportado tras su revisión. | UR-10 | — | Vigente |
| FR-138 | El sistema debe permitir al coordinador notificar al autor del contenido sobre la acción tomada, incluyendo los motivos de la decisión. | UR-10 | — | Vigente |
| FR-139 | El sistema debe permitir al coordinador restaurar contenido previamente eliminado o bloqueado si se determina que el reporte no era válido. | UR-10 | — | Vigente |
| FR-142 | El sistema debe permitir a los usuarios cuyos contenidos hayan sido eliminados apelar la decisión mediante un formulario de apelación accesible desde su perfil. | UR-10 | — | Vigente |
| FR-145 | El sistema debe enviar alertas internas a los coordinadores cuando se detecte contenido con múltiples reportes en un corto período de tiempo. | UR-10 | — | Vigente |
| FR-146 | El sistema debe registrar todas las acciones de moderación realizadas, incluyendo la fecha, el coordinador responsable y el detalle de la acción, para fines de auditoría. | UR-10 | — | Vigente |
| FR-147 | El sistema debe garantizar que el contenido eliminado no sea accesible para los usuarios después de ser retirado. | UR-10 | — | Vigente |
| FR-148 | El sistema debe proporcionar a los coordinadores estadísticas sobre los reportes recibidos, incluyendo volumen por categoría, tendencias y reincidencias de usuarios. | UR-10 | — | Vigente |
| FR-149 | El sistema debe permitir a los coordinadores asignar roles de moderación a usuarios autorizados para colaborar en la gestión del contenido. | UR-10 | — | Retirado |
| FR-150 | El sistema debe permitir al coordinador definir y actualizar las reglas de moderación y los criterios de bloqueo automático de contenido. | UR-10 | — | Vigente |
| FR-151 | El sistema debe soportar moderación multilingüe, permitiendo detectar y gestionar contenido en diferentes idiomas soportados por la plataforma. | UR-10 | — | Vigente |
| FR-152 | El sistema debe permitir a coordinadores y moderadores gestionar reportes y contenido desde dispositivos de escritorio y móviles. | UR-10 | — | Vigente |
| FR-153 | El sistema debe permitir al usuario registrado valorar recetas mediante un sistema de estrellas de 1 a 5. | UR-11 | — | Vigente |
| FR-154 | El sistema debe mostrar la calificación promedio de cada receta, calculada automáticamente a partir de todas las valoraciones recibidas. | UR-11 | — | Vigente |
| FR-155 | El sistema debe mostrar el número total de valoraciones que ha recibido cada receta, visible en la vista previa y detallada. | UR-11 | — | Vigente |
| FR-156 | El sistema debe permitir al usuario registrado comentar en las recetas, con un límite de 500 caracteres por comentario. | UR-11 | — | Vigente |
| FR-157 | El sistema debe mostrar el número total de comentarios que ha recibido cada receta, visible en la vista previa y detallada. | UR-11 | — | Vigente |
| FR-158 | El sistema debe permitir al usuario editar sus propios comentarios dentro de los 15 minutos posteriores a su publicación. | UR-11 | — | Vigente |
| FR-159 | El sistema debe permitir al usuario eliminar permanentemente sus propios comentarios en cualquier momento. | UR-11 | — | Vigente |
| FR-160 | El sistema debe notificar al autor de la receta cuando un usuario la valore o comente. | UR-11 | — | Vigente |
| FR-161 | El sistema debe evitar que un usuario emita más de una valoración sobre una misma receta, permitiendo solo una valoración por receta por usuario. | UR-11 | — | Vigente |
| FR-162 | El sistema debe permitir al usuario responder a comentarios de otros usuarios en recetas, mostrando la relación jerárquica entre comentario y respuesta. | UR-11 | — | Vigente |
| FR-163 | El sistema debe notificar al usuario cuando alguien responda a uno de sus comentarios en recetas. | UR-11 | — | Vigente |
| FR-164 | El sistema debe permitir al usuario reportar comentarios inapropiados mediante una opción visible en cada comentario. *(conecta con UR-09)* | UR-11 | — | Vigente |
| FR-165 | El sistema debe mostrar una sección de "Recetas mejor valoradas", destacando aquellas con calificación más alta en cada categoría de búsqueda. | UR-11 | — | Vigente |
| FR-166 | El sistema debe actualizar en tiempo real las valoraciones y comentarios de las recetas, reflejando inmediatamente nuevas interacciones. | UR-11 | — | Vigente |
| FR-167 | El sistema debe integrar las valoraciones en el algoritmo de recomendación, priorizando recetas altamente valoradas que coincidan con las preferencias del usuario. | UR-11 | — | Vigente |
| FR-168 | El sistema debe permitir al usuario marcar comentarios como "útiles" o "no útiles", mostrando un contador visible en cada comentario. | UR-11 | — | Vigente |
| FR-169 | El sistema debe mostrar la fecha y hora exacta de cada comentario y valoración, visible junto al contenido correspondiente. | UR-11 | — | Vigente |
| FR-170 | El sistema debe mostrar solo el alias asociado a cada valoración y comentario, sin exponer datos personales adicionales. | UR-11 | — | Vigente |
| FR-171 | El sistema debe mostrar una sección de "Comentarios destacados", resaltando aquellos marcados como útiles por varios usuarios. | UR-11 | — | Vigente |
| FR-172 | El sistema debe ofrecer una guía interactiva accesible en cualquier momento desde todas las páginas de la plataforma mediante un botón o enlace claramente visible. | UR-12 | — | Vigente |
| FR-173 | El sistema debe proporcionar en la guía interactiva instrucciones paso a paso sobre las funcionalidades de la plataforma, como registro, inicio de sesión, búsqueda y publicación de recetas, uso del foro, valoración y comentarios. | UR-12 | — | Vigente |
| FR-174 | El sistema debe mostrar la guía interactiva de manera contextual, ofreciendo ayuda específica según la sección de la plataforma en la que se encuentre el usuario. | UR-12 | — | Vigente |
| FR-175 | El sistema debe permitir al usuario navegar libremente entre los distintos módulos o temas de la guía interactiva. | UR-12 | — | Vigente |
| FR-176 | El sistema debe mostrar elementos visuales en la guía interactiva, como resaltados, flechas o ventanas emergentes, que señalen las partes relevantes de la interfaz. | UR-12 | — | Vigente |
| FR-177 | El sistema debe permitir al usuario pausar, reanudar o salir de la guía interactiva en cualquier momento. | UR-12 | — | Vigente |
| FR-178 | El sistema debe registrar el progreso del usuario en la guía interactiva, permitiéndole reanudar desde el punto donde la dejó en sesiones anteriores. | UR-12 | — | Vigente |
| FR-179 | El sistema debe incluir en la guía interactiva tutoriales multimedia, como videos o animaciones, para explicar funcionalidades de la plataforma. | UR-12 | — | Vigente |
| FR-180 | El sistema debe permitir al usuario buscar temas específicos dentro de la guía interactiva mediante palabras clave. | UR-12 | — | Vigente |
| FR-181 | El sistema debe permitir al coordinador aprobar nuevas cuentas de cuidador y de nutricionista desde el panel de gestión de inscripciones. | UR-13 | — | Vigente |
| FR-182 | El sistema debe permitir al coordinador suspender cuentas de usuario activas desde el panel de gestión de inscripciones. | UR-13 | — | Vigente |
| FR-183 | El sistema debe permitir al coordinador eliminar cuentas de usuario desde el panel de gestión de inscripciones. | UR-13 | — | Vigente |
| FR-184 | El sistema debe permitir al coordinador visualizar un listado de todas las cuentas de usuario, con información básica (nombre, correo, rol y estado de la cuenta). | UR-13 | — | Vigente |
| FR-185 | El sistema debe registrar la fecha, hora y acción realizada cada vez que el coordinador apruebe, suspenda o elimine una cuenta, manteniendo un historial de auditoría. | UR-13 | — | Vigente |
| FR-186 | El sistema debe permitir al coordinador bloquear temporalmente a un usuario que viole las políticas de la plataforma, especificando la duración del bloqueo. | UR-13 | — | Vigente |
| FR-187 | El sistema debe permitir al coordinador expulsar permanentemente a un usuario por infracciones graves, impidiendo su acceso al sistema. | UR-13 | — | Vigente |
| FR-207 | El sistema debe ofrecer, en el primer acceso del usuario, un recorrido de bienvenida que pueda omitirse, independiente de la ayuda contextual disponible en cada pantalla. | UR-12 | — | Vigente |
| FR-208 | El sistema debe retirar al cuidador el acceso a la información de un paciente cuando deje de estar asociado a él. | UR-13 | — | Vigente |
| FR-209 | El sistema debe marcar como inactiva la cuenta de un cuidador que, transcurridos tres meses, no esté asociada a ningún paciente. | UR-13 | — | Vigente |
| FR-210 | El sistema debe eliminar automáticamente la cuenta de un cuidador que permanezca sin asociación a ningún paciente durante un año completo. | UR-13 | — | Vigente |
| FR-211 | El sistema debe conservar el contenido publicado por un cuidador tras la eliminación de su cuenta. | UR-13 | — | Vigente |
| FR-212 | El sistema debe permitir que una misma cuenta reúna varios de los perfiles de paciente, cuidador, nutricionista y coordinador, conservando las condiciones de habilitación de cada perfil. | UR-13 | — | Vigente |
| FR-198 | El sistema debe permitir al paciente revocar, en cualquier momento, el acceso previamente concedido a un nutricionista sobre sus datos fisiológicos y de salud. | UR-05 | — | Vigente |
| FR-199 | El sistema debe permitir al nutricionista autorizado proponer al paciente una frecuencia para sus recordatorios de registro de datos. | UR-05 | — | Vigente |
| FR-200 | El sistema debe mantener un recordatorio como pendiente hasta que el paciente complete o descarte el registro de datos asociado. | UR-05 | — | Vigente |
| FR-201 | El sistema debe permitir al paciente autorizar a su cuidador el acceso a los datos de salud que decida compartir. | UR-05 | — | Vigente |
| FR-202 | El sistema debe registrar, para cada cambio de umbral crítico, la fecha, el autor del cambio y el momento desde el que se aplica. | UR-05 | — | Vigente |
| FR-203 | El sistema debe notificar al paciente cuando se modifique un umbral crítico aplicable a sus datos. | UR-05 | — | Vigente |
| FR-204 | El sistema debe permitir al paciente o al cuidador proponer una receta creada, quedando esta en estado pendiente de validación hasta su revisión por un nutricionista. | UR-06 | — | Vigente |
| FR-205 | El sistema debe permitir al nutricionista validar una receta propuesta por un paciente o un cuidador, tras lo cual la receta se publica como validada. | UR-06 | — | Vigente |
| FR-206 | El sistema debe mostrar, junto al nombre del nutricionista, un distintivo visual (por ejemplo, una estrella u otro icono) en sus intervenciones y publicaciones del foro y en sus consejos de vida saludable. | UR-07 | — | Vigente |
| FR-216 | El sistema debe permitir al paciente filtrar su historial de datos fisiológicos por tipo de dato. | UR-05 | — | Vigente |
| FR-217 | El sistema debe notificar al paciente cuando se genere una alerta crítica, mostrando un mensaje que sugiera explícitamente buscar atención médica. | UR-05 | — | Vigente |
| FR-195 | El sistema debe permitir a cualquier persona, sin necesidad de registro, consultar el foro y su contenido. | UR-04 | — | Vigente |
| FR-196 | El sistema debe permitir el envío de mensajes directos entre usuarios registrados. | UR-04 | — | Vigente |
| FR-197 | El sistema debe permitir a un usuario registrado seguir a otros usuarios, con independencia del seguimiento de hilos ya previsto en FR-029. | UR-04 | — | Vigente |
| FR-188 | El sistema debe requerir, durante el registro, un alias único, distinto del nombre completo del usuario, con un mínimo de tres caracteres, sin espacios, pudiendo incluir guion o guion bajo. | UR-01 | — | Vigente |
| FR-189 | El sistema debe proponer alias alternativos cuando el solicitado ya esté en uso, sin impedir que el usuario introduzca manualmente un alias distinto. | UR-01 | — | Vigente |
| FR-190 | El sistema debe vincular automáticamente una cuenta local y una cuenta de Google cuando ambas correspondan al mismo correo electrónico. | UR-01 | — | Vigente |
| FR-191 | El sistema debe restringir las funciones de publicación profesional de una cuenta registrada como nutricionista a las disponibles para un usuario general mientras su documentación no haya sido aprobada por el coordinador. | UR-01 | — | Vigente |
| FR-192 | El sistema debe mostrar el alias del usuario, y no su nombre completo, como identidad visible en el foro y demás espacios públicos de la plataforma. | UR-01 | — | Vigente |
| FR-193 | El sistema debe permitir a quien se registre como cuidador indicar el paciente o los pacientes a quienes cuidará. | UR-01 | — | Vigente |
| FR-194 | El sistema debe requerir la autorización expresa de cada paciente antes de activar la relación de cuidado correspondiente. | UR-01 | — | Vigente |
| FR-213 | El sistema debe validar el formato y el tamaño del archivo de documentación profesional antes de continuar con el registro, mostrando junto al campo de carga cualquier error detectado. | UR-01 | — | Vigente |
| FR-214 | El sistema debe mostrar, mientras la cuenta esté pendiente de verificación del correo electrónico, una pantalla que indique que el registro no se ha completado. | UR-01 | — | Vigente |
| FR-215 | El sistema debe impedir finalizar el registro si alguna de las dos casillas de aceptación —términos y condiciones, política de privacidad— no está marcada. | UR-01 | — | Vigente |
| FR-218 | El sistema debe mantener una única cuenta personal de Simbiosis, de uso individual, por cada persona registrada, con independencia de sus modalidades de acceso. | UR-01 | — | Vigente |
| FR-219 | El sistema debe admitir, para cada paciente, ninguna o una única relación de cuidado activa. | UR-01, UR-13 | — | Vigente |
| FR-220 | El sistema debe permitir seleccionar y editar preferencias dietéticas únicamente a usuarios con perfil de paciente. | UR-03 | — | Vigente |

FR-017 se conserva para no perder el identificador histórico, pero su estado es `Retirado`: la autenticación de dos factores queda excluida de esta fase.

FR-149 se conserva para no perder el identificador histórico, pero su estado es `Retirado`: el [apartado 4 del acta de captura de requisitos generales](../captura/acta-captura-requisitos-generales.md#4-foro-interacción-y-moderación) establece que el coordinador es el único rol responsable de administrar y moderar el foro.

## 5. Requisitos no funcionales

| ID | Categoría y atributo | Requisito no funcional | Ámbito | UR/FR relacionados | Fuente | Método de comprobación | Estado |
| --- | --- | --- | --- | --- | --- | --- | --- |
| NFR-001 | NFR-Q · Disponibilidad | La plataforma alcanzará una disponibilidad mínima del 99,5 % en cada mes natural, medida mediante comprobaciones externas cada cinco minutos. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.1.4 | Revisar las comprobaciones externas de cada cinco minutos y calcular la disponibilidad mensual conforme al acta. | Vigente |
| NFR-002 | NFR-Q · Integridad | La plataforma realizará al menos una copia de seguridad diaria de la información de salud y de las recetas. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.2.1; [Documento de Visión y Alcance](../vision/vision_y_alcance.md), §3.3 | Revisar el registro de copias de seguridad y comprobar que no falte ninguna copia diaria. | Vigente |
| NFR-003 | NFR-Q · Localización e internacionalización | La primera versión estará disponible en castellano y gallego. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.4.4; [acta de captura de requisitos generales](../captura/acta-captura-requisitos-generales.md), §7.2 | Revisar todas las pantallas y mensajes de la primera versión en ambos idiomas. | Vigente |
| NFR-004 | NFR-Q · Capacidad y escalabilidad | La plataforma soportará una carga de 100 usuarios concurrentes y 10 operaciones por segundo durante 30 minutos. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.1.1 y §2.1.2 | Ejecutar una prueba de carga con 100 usuarios concurrentes y 10 operaciones por segundo durante 30 minutos. | Vigente |
| NFR-005 | NFR-Q · Rendimiento | Con la carga de NFR-004, el 95 % de los inicios de sesión y de las consultas definidas para la prueba se completará en un máximo de 2 segundos. | Local | UR-02, UR-03, UR-04, UR-08 | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.1.2 y §2.1.3 | Medir los tiempos del 95 % de las operaciones indicadas durante la prueba de NFR-004, con los límites de medición del acta. | Vigente |
| NFR-006 | NFR-Q · Rendimiento | Con la carga de NFR-004, el 95 % de las publicaciones de recetas, comentarios o mensajes se completará en un máximo de 3 segundos. | Local | UR-04, UR-06, UR-11 | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.1.2 y §2.1.3 | Medir los tiempos del 95 % de las operaciones indicadas durante la prueba de NFR-004, con los límites de medición del acta. | Vigente |
| NFR-007 | NFR-Q · Rendimiento y Mantenibilidad | La plataforma mantendrá los objetivos de capacidad y rendimiento definidos para la primera versión sin intervención manual del personal de la organización. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.1.1 | Ejecutar la prueba de carga de NFR-004 y comprobar en los registros el ajuste automático de recursos y la ausencia de intervención manual del personal de la organización. | Vigente |
| NFR-008 | NFR-Q · Recuperabilidad | Tras un incidente grave, la plataforma recuperará las funciones principales en un máximo de cuatro horas desde la declaración del incidente. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.2.1 | Probar la recuperación tras un incidente grave y medir el tiempo desde su declaración hasta la recuperación de las funciones principales. | Vigente |
| NFR-009 | NFR-Q · Integridad | Tras un incidente grave, la pérdida de información no superará la correspondiente a las 24 horas anteriores al incidente. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.2.1 | Restaurar una copia tras un incidente simulado y comprobar la antigüedad de la información recuperada. | Vigente |
| NFR-010 | NFR-Q · Accesibilidad | Todas las pantallas y funciones de la primera versión cumplirán el estándar WCAG 2.2, nivel AA. La conformidad se revisará antes de aceptar la versión y después de cambios importantes de interfaz. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.4.2 y §2.4.3 | Combinar una herramienta automática y una revisión manual de los recorridos indicados en el acta. | Vigente |
| NFR-011 | NFR-R · Plataforma | El acceso a la plataforma se realizará mediante una interfaz web responsiva y no requerirá la instalación de una aplicación nativa o de escritorio en el dispositivo cliente. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.5.1; [SRS](./srs.md), §1.3 y §2.3 | Revisar la arquitectura y comprobar el acceso desde navegadores compatibles sin instalación adicional. | Vigente |
| NFR-012 | NFR-R · Despliegue | La plataforma se desplegará en una infraestructura en la nube gestionada por un proveedor externo. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.5.2; [SRS](./srs.md), §2.4; [Documento de Visión y Alcance](../vision/vision_y_alcance.md), §3.3 | Revisar la arquitectura y la configuración del despliegue. | Vigente |
| NFR-013 | NFR-R · Tecnología web | La interfaz cliente se implementará utilizando estándares web abiertos —HTML5, CSS y ECMAScript— y no dependerá de plugins propietarios ni requerirá la instalación de software adicional en el dispositivo de la persona usuaria. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.5.1 | Revisar las dependencias del cliente y comprobar el acceso sin plugins ni software adicional. | Vigente |
| NFR-014 | NFR-I · Interfaz de usuario y localización | La interfaz permitirá cambiar entre castellano y gallego. Al seleccionar un idioma, los textos de navegación, formularios, validaciones y mensajes de la interfaz se mostrarán íntegramente en ese idioma. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.4.4; [acta de captura de requisitos generales](../captura/acta-captura-requisitos-generales.md), §7.2; [SRS](./srs.md), §7 | Cambiar el idioma y revisar todas las pantallas y mensajes de la primera versión en ambos idiomas. | Vigente |
| NFR-015 | NFR-I · Interfaz de software y autenticación | La autenticación mediante una cuenta de Google utilizará OAuth 2.0 u OpenID Connect sobre HTTPS y la plataforma no almacenará la contraseña de Google. | Global | — | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.3.1; [SRS](./srs.md), §5.2 | Probar la autenticación con una cuenta de prueba y revisar la configuración de la integración. | Vigente |

Las relaciones de NFR-005 y NFR-006 se registran por UR. Su aplicación se limita a las operaciones siguientes, definidas en el [acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.1.2:

| NFR | UR relacionado | Operaciones cubiertas |
| --- | --- | --- |
| NFR-005 | UR-02 | Inicio de sesión. |
| NFR-005 | UR-03 | Consulta del perfil. |
| NFR-005 | UR-04 | Consulta del foro. |
| NFR-005 | UR-08 | Búsqueda y consulta de recetas. |
| NFR-006 | UR-04 | Publicación de hilos, comentarios y respuestas en el foro. |
| NFR-006 | UR-06 | Publicación de recetas. |
| NFR-006 | UR-11 | Publicación de comentarios y respuestas en recetas. |

El enlace a un UR no extiende el objetivo temporal a todas sus funciones. Se mantienen la carga de NFR-004, el porcentaje y el tiempo de cada NFR y los límites de medición del acta, §2.1.3.

`NFR-Q` identifica atributos de calidad; `NFR-R`, restricciones de diseño e implementación; y `NFR-I`, requisitos de interfaz externa.

Categorías y atributos:

1. Requisitos de calidad (NFR-Q): Rendimiento, Usabilidad, Seguridad, Fiabilidad, Disponibilidad, Modificabilidad, Portabilidad, Eficiencia, Escalabilidad, Verificabilidad / Testabilidad, Robustez, Seguridad funcional (safety), Integridad, Reusabilidad, Instalabilidad.
2. Restricciones (NFR-R): Tecnología y entorno, Hardware, Regulaciones y estándares, Compatibilidad, Interfaces existentes, Restricciones presupuestarias y de gestión.
3. Requisitos de interfaz externa (NFR-I): Interfaz de usuario, Interfaz de software, Interfaz de hardware, Interfaz de comunicación.

## 6. Matriz de trazabilidad

| UR | FR asociados | NFR globales o ligados | UC relacionados |
| --- | --- | --- | --- |
| UR-01 | FR-001, FR-002, FR-003, FR-004, FR-005, FR-006, FR-007, FR-008, FR-009, FR-010, FR-011, FR-012, FR-013, FR-014, FR-188, FR-189, FR-190, FR-191, FR-192, FR-193, FR-194, FR-213, FR-214, FR-215, FR-218, FR-219 | — | — |
| UR-02 | FR-015, FR-016, FR-017, FR-018 | NFR-005 | — |
| UR-03 | FR-019, FR-020, FR-220 | NFR-005 | — |
| UR-04 | FR-021, FR-022, FR-023, FR-024, FR-025, FR-026, FR-027, FR-028, FR-029, FR-030, FR-031, FR-032, FR-033, FR-034, FR-035, FR-036, FR-037, FR-038, FR-039, FR-040, FR-195, FR-196, FR-197 | NFR-005, NFR-006 | — |
| UR-05 | FR-041, FR-042, FR-043, FR-044, FR-045, FR-046, FR-047, FR-048, FR-049, FR-050, FR-051, FR-052, FR-053, FR-198, FR-199, FR-200, FR-201, FR-202, FR-203, FR-216, FR-217 | — | — |
| UR-06 | FR-054, FR-055, FR-056, FR-057, FR-058, FR-059, FR-060, FR-061, FR-062, FR-063, FR-064, FR-065, FR-066, FR-204, FR-205 | NFR-006 | — |
| UR-07 | FR-067, FR-068, FR-069, FR-070, FR-071, FR-072, FR-073, FR-074, FR-075, FR-076, FR-077, FR-078, FR-079, FR-080, FR-081, FR-082, FR-083, FR-084, FR-206 | — | — |
| UR-08 | FR-085, FR-086, FR-087, FR-088, FR-089, FR-090, FR-091, FR-092, FR-093, FR-094, FR-095, FR-096, FR-097, FR-098, FR-099, FR-100, FR-101, FR-102, FR-103, FR-104, FR-105, FR-106, FR-107, FR-108, FR-109, FR-110, FR-111, FR-112, FR-113, FR-114, FR-115, FR-116, FR-117, FR-118, FR-119 | NFR-005 | — |
| UR-09 | FR-120, FR-121, FR-122, FR-123, FR-124, FR-125, FR-126 | — | — |
| UR-10 | FR-127, FR-128, FR-129, FR-130, FR-131, FR-132, FR-133, FR-134, FR-135, FR-136, FR-137, FR-138, FR-139, FR-142, FR-145, FR-146, FR-147, FR-148, FR-149, FR-150, FR-151, FR-152 | — | — |
| UR-11 | FR-153, FR-154, FR-155, FR-156, FR-157, FR-158, FR-159, FR-160, FR-161, FR-162, FR-163, FR-164, FR-165, FR-166, FR-167, FR-168, FR-169, FR-170, FR-171 | NFR-006 | — |
| UR-12 | FR-172, FR-173, FR-174, FR-175, FR-176, FR-177, FR-178, FR-179, FR-180, FR-207 | — | — |
| UR-13 | FR-181, FR-182, FR-183, FR-184, FR-185, FR-186, FR-187, FR-208, FR-209, FR-210, FR-211, FR-212, FR-219 | — | — |

## 7. Control de cambios

Los identificadores no se reutilizan ni se renumeran. Cuando se acepta un cambio, se conserva la identidad del requisito si mantiene el mismo significado; si aparece una necesidad nueva, se asigna un identificador nuevo.

| Versión | Fecha | Cambios | Requisitos afectados | Fuente o evidencia |
| --- | --- | --- | --- | --- |
| 1.16 | 19/11/2026 | Se limitan las preferencias dietéticas a pacientes y se ajustan UC-05 y la recomendación basada en preferencias alimenticias. | FR-019, FR-104, FR-220; UR-03 | [Acta de información del dominio](../captura/acta-acuerdos-informacion-dominio.md#91-gestión-de-usuarios); SC-002 |
| 1.15 | 19/11/2026 | Se confirma una cuenta personal única por persona, se amplía la compatibilidad de perfiles y se limita a uno el cuidador activo de cada paciente, que también puede no tener cuidador. Se actualizan las asociaciones por UR y la matriz. | FR-212, FR-218 y FR-219; UR-01 y UR-13 | [Acta de información del dominio](../captura/acta-acuerdos-informacion-dominio.md#91-gestión-de-usuarios); [SC-001](../cambios/registro-solicitudes-cambio.md#solicitudes) y [DEC-001](../decisiones/registro-decisiones.md#decisiones) |
| 1.14 | 15/10/2026 | Se completan los enlaces por UR de NFR-005 y NFR-006 y su relación inversa en la matriz. Se delimita cada relación por las operaciones cubiertas, sin cambiar los objetivos de rendimiento ni las condiciones de medición. | NFR-005, NFR-006; UR-02, UR-03, UR-04, UR-06, UR-08 y UR-11 | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md), §2.1.2 y §2.1.3 |
| 1.13 | 02/10/2026 | Se añade un índice con enlaces a los apartados del catálogo. | — | Mejora de navegación |
| 1.12 | 02/10/2026 | Se incorporan los quince NFR de la primera versión, con ámbito, procedencia y método de comprobación. NFR-007 se clasifica como Rendimiento y Mantenibilidad. | NFR-001–NFR-015 | [Acta de acuerdos técnicos y operativos](../captura/acta-acuerdos-tecnicos-operativos.md) |
| 1.11 | 24/09/2026 | Se retira FR-149 por ser incompatible con la responsabilidad exclusiva del coordinador en la administración y moderación del foro. | FR-149 | [Acta de captura de requisitos generales, apartado 4](../captura/acta-captura-requisitos-generales.md#4-foro-interacción-y-moderación) |
| 1.10 | 23/09/2026 | Se sustituyen los intervalos por enumeraciones explícitas de FR en las asociaciones de los UR y en la matriz de trazabilidad. | UR-01–UR-13 | Mejora de legibilidad del catálogo |
| 1.9 | 23/09/2026 | Se declara consolidada la base funcional de partida: contiene los UR y FR canónicos y mantiene los NFR pendientes. | UR-01–UR-13, FR-001–FR-217 | Catálogo canónico de requisitos, v2.0 |
| 1.8 | 22/09/2026 | Se actualizan las asociaciones BO–UR en el catálogo. | BO-01–BO-06, UR-04–UR-13 | Análisis de trazabilidad del catálogo |
| 1.7 | 22/09/2026 | Se añaden asociaciones BO–UR a partir del significado de los objetivos y del alcance del proyecto. | BO-01–BO-06, UR-04–UR-13 | Análisis de trazabilidad del catálogo |
| 1.6 | 22/09/2026 | Se incorporan UR-12 y UR-13 con sus 22 FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-12, UR-13, FR-172–FR-187, FR-207–FR-212 | Catálogo canónico de requisitos, v2.0 |
| 1.5 | 22/09/2026 | Se incorpora UR-11 y sus 19 FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-11, FR-153–FR-171 | Catálogo canónico de requisitos, v2.0 |
| 1.4 | 22/09/2026 | Se incorpora UR-10 y sus 22 FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-10, FR-127–FR-139, FR-142, FR-145–FR-152 | Catálogo canónico de requisitos, v2.0 |
| 1.3 | 22/09/2026 | Se incorpora UR-09 y sus 7 FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-09, FR-120–FR-126 | Catálogo canónico de requisitos, v2.0 |
| 1.2 | 22/09/2026 | Se incorpora UR-08 y sus 35 FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-08, FR-085–FR-119 | Catálogo canónico de requisitos, v2.0 |
| 1.1 | 22/09/2026 | Se incorpora UR-07 y sus 19 FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-07, FR-067–FR-084, FR-206 | Catálogo canónico de requisitos, v2.0 |
| 1.0 | 22/09/2026 | Se incorpora UR-06 y sus 15 FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-06, FR-054–FR-066, FR-204–FR-205 | Catálogo canónico de requisitos, v2.0 |
| 0.9 | 22/09/2026 | Se incorpora UR-05 y sus 21 FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-05, FR-041–FR-053, FR-198–FR-203, FR-216–FR-217 | Catálogo canónico de requisitos, v2.0 |
| 0.8 | 22/09/2026 | Se incorpora UR-04 y sus 23 FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-04, FR-021–FR-040, FR-195–FR-197 | Catálogo canónico de requisitos, v2.0 |
| 0.7 | 22/09/2026 | Se incorpora UR-03 y sus dos FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-03, FR-019, FR-020 | Catálogo canónico de requisitos, v2.0 |
| 0.6 | 22/09/2026 | Se incorpora FR-017 como registro histórico con estado `Retirado`, en lugar de omitirlo del catálogo. | UR-02, FR-017 | Catálogo canónico de requisitos, v2.0 |
| 0.5 | 22/09/2026 | Se incorpora UR-02 y sus tres FR vigentes; se deja constancia de que FR-017 está retirado en el catálogo canónico v2.0. | UR-02, FR-015, FR-016, FR-018 | Catálogo canónico de requisitos, v2.0 |
| 0.4 | 22/09/2026 | Se incorporan literalmente los seis objetivos de negocio del Documento de Visión y Alcance vigente, versión 2.4. | BO-01–BO-06 | [Documento de Visión y Alcance](../vision/vision_y_alcance.md), v2.4 |
| 0.3 | 22/09/2026 | Se elimina la columna `Fuente` de las tablas de requisitos; la referencia común queda en la cabecera y la procedencia de cambios en este historial. | — | Decisión de estructura del catálogo |
| 0.2 | 22/09/2026 | Se incorpora UR-01 y sus 24 FR asociados, volcados desde el catálogo canónico de Notion v2.0. | UR-01, FR-001–FR-014, FR-188–FR-194, FR-213–FR-215 | Catálogo canónico de requisitos, v2.0 |
| 0.1 | 22/09/2026 | Se crea la plantilla inicial. | — | Decisión de estructura de la SRS |
