# Proyecto Simbiosis — Repositorio Documental

Repositorio de ejemplo para la gestión profesional de requisitos del proyecto ficticio **Proyecto Simbiosis**. Su finalidad es servir de referencia docente sobre cómo organizar, versionar y revisar la documentación de un proyecto de ingeniería del software.

## Fuente canónica

Todos los documentos propios del proyecto se redactan y mantienen en **Markdown** dentro de este repositorio. Los archivos en Markdown son la fuente de verdad; cualquier exportación a otro formato (PDF u otros) es una copia derivada, no editable, publicada en [`releases/`](releases/README.md).

## Líneas base

Una línea base (versión estable de la documentación) se declara mediante:

- Una **etiqueta (tag) de Git** sobre el commit correspondiente.
- Una entrada correspondiente en [`CHANGELOG.md`](CHANGELOG.md) que describe el alcance de esa línea base.

Los nombres de archivo no incluyen números de versión: el histórico y las versiones los gestionan Git y las etiquetas.

## Estructura del repositorio

```
├── README.md                  Este documento
├── CHANGELOG.md                Historial de líneas base
├── docs/
│   ├── vision/                 Visión y alcance del proyecto
│   ├── captura/                 Actas de captura y aclaración de requisitos
│   ├── decisiones/              Registro de decisiones
│   ├── requisitos/              SRS y catálogo de requisitos
│   ├── calidad/                  Criterios de revisión de requisitos
│   ├── cambios/                  Registro de solicitudes de cambio
│   ├── planificacion/            Planes y evaluaciones de iteración
│   ├── modelos/                  Modelos y diagramas del proyecto
│   └── referencias/              Documentos externos o recibidos (no editables)
└── releases/                    Versiones estables exportadas (p. ej. PDF)
```

Los planes de [E1](docs/planificacion/plan-iteracion-e1.md), [E2](docs/planificacion/plan-iteracion-e2.md) y [E3](docs/planificacion/plan-iteracion-e3.md) definen el alcance funcional y el trabajo previsto de tres iteraciones simuladas de Elaboración. E1 aborda acceso, cuentas y ayuda. E2 amplía el trabajo con salud y recetas. E3 incorpora el foro y la resolución de reportes sobre su contenido.

## Convenciones

- Nombres de archivo en minúsculas y con guiones.
- Sin versiones en los nombres de archivo.
- `docs/referencias/` contiene únicamente material externo o recibido; los documentos propios viven en las demás carpetas de `docs/`.
- `releases/` contiene solo exportaciones estables; no es la fuente editable.
