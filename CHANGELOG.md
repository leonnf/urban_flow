
# CHANGELOG — Sprint 3

## [Sprint 3] - Junio 2026

### Ejercicio 01-02: Inicialización y DVC
- Configuración de rama Sprint_3
- Inicialización de DVC con remote local
- Migración de CSV e imágenes a DVC
- Creación de archivos `.dvc`

### Ejercicio 03-04: Modelos y funciones
- Diseño del modelo lógico entidad-relación
- Definición de clases simples (Vehículo, Radar, Multa, Evidencia)
- Implementación de función procesar_fila_csv()
- Validación de mapeo de datos

### Ejercicio 05-06: Base de datos relacional
- Implementación de modelos SQLAlchemy
- Creación de BD SQLite (transito.db)
- Población de tablas (969 multas, 66 vehículos, 3 radares)
- Inserción de 103 evidencias vinculadas

### Ejercicio 07: Consultas SQL
- Top 10 patentes más multadas
- Multas sin evidencia
- Radares más activos
- Reincidentes por período
- Estadísticas de cobertura visual
- Almacenamiento de consultas en archivo

### Ejercicio 08-09: Base de datos vectorial
- Inicialización de ChromaDB persistente
- Vectorización de imágenes con OpenClip
- Mapeo imagen → vehículo
- Procesamiento de 25 imágenes únicas
- Función buscar_patente_imagen() con similitud corregida
- Búsqueda por similitud visual

### Ejercicio 10: Conclusiones y documentación
- Redacción de conclusiones en data/Readme.md
- Creación de README.md general
- Creación de CHANGELOG.md
- Actualización de datos según resultados reales

## Resumen de cambios técnicos

- **BD Relacional:** SQLite con 4 entidades, 969 registros
- **BD Vectorial:** ChromaDB con 25 imágenes vectorizadas
- **Versionado:** DVC para datos grandes
- **Similitud:** Corregida para rango 0-1 (antes tenía valores negativos)
- **Cobertura:** 10.63% de multas con evidencia visual

## Próximos pasos

- Implementar predicción de reincidencia
- Mejorar cobertura de evidencias visuales
- Optimizar búsqueda vectorial con más imágenes
