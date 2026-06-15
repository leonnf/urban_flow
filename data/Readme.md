
## Conclusiones — Sprint 3

### Cobertura de Evidencia Visual

El análisis del dataset de multas de tránsito revela que de las 969 infracciones registradas, solo 103 cuentan con evidencia visual confirmada, lo que representa el 10.63% de cobertura. Las 866 multas restantes (89.37%) carecen de evidencia fotográfica.

- **Total de multas:** 969
- **Multas con evidencia:** 103
- **Multas sin evidencia:** 866
- **Porcentaje confirmado visualmente:** 10.63%
- **Imágenes únicas vectorizadas en ChromaDB:** 25

### Patentes con Mayor Reincidencia

Se identificó que las patentes con mayor cantidad de infracciones concentran un patrón significativo de violaciones. La patente más multada registró 22 infracciones, siendo las tres principales:

- **UM96201:** 22 infracciones
- **T0YDR:** 22 infracciones
- **TL03GOG:** 21 infracciones

### Actividad de Radares

Los puntos de control generaron una distribución desigual de multas. Los tres radares más activos registraron entre 319 y 328 infracciones cada uno:

- **AV SIEMPRE VIVA:** 328 multas
- **AV LIBERTADOR:** 322 multas
- **AV LIBERTADOR:** 319 multas

### Implementación Técnica

Se desarrolló una solución completa que integra:
- Base de datos relacional SQLite con 4 entidades (Vehículo, Radar, Multa, Evidencia)
- Migración de datos a DVC para control de versiones
- Base de datos vectorial ChromaDB con 25 imágenes de patentes vectorizadas
- Búsqueda por similitud usando OpenClip ViT-B-32 para identificación visual

### Conclusiones Finales

La solución implementada permite:
1. Rastrear infracciones por vehículo y detectar patrones de reincidencia
2. Analizar la actividad de cada punto de control de tránsito
3. Buscar vehículos por similitud visual de patente
4. Mantener datos versionados con control de cambios mediante DVC
5. Proporcionar una base para análisis predictivo y enforcement de tránsito
