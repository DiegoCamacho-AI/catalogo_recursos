# Catálogo de Recursos Académicos

Estructura inicial de un sistema para registrar y consultar recursos académicos
(libros, sitios web, videos, artículos y herramientas de software).

## Objetivo
Sentar las bases de un catálogo que en versiones futuras permitirá registrar,
clasificar y consultar recursos académicos de distinto tipo.

## Estructura del proyecto
- `app/` - código fuente de la aplicación
- `data/` - datos del catálogo (recursos.json)
- `docs/` - documentación y evidencias del proceso
- `tests/` - pruebas básicas

## Tecnologías
- Python 3.x
- requests
- rich

## Preparar el entorno
1. Crear entorno virtual: `python -m venv .venv`
2. Activarlo
3. Instalar dependencias: `pip install -r requirements.txt`

## Dependencias
Ver `requirements.txt`

## Próximas mejoras

- Implementar el registro y edición de recursos desde la aplicación.
- Agregar búsqueda y filtrado por tipo, tema, nivel o autor.
- Incorporar pruebas automatizadas más completas en `tests/`.
- Conectar el catálogo a una fuente de datos externa mediante `requests`.
