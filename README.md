# Sistema de Inventario de Equipos - Escorial

## Descripción
Sistema de información para controlar la entrega, devolución y reemplazo de equipos de sistemas (PC, teclados, monitores, etc.) entregados a los empleados de Escorial, relacionando cada elemento con su número de serie y con el empleado a cargo.

Proyecto de la materia Organización Empresarial, Tecnicatura Universitaria en Programación (UTN).

## Integrantes
- Lautaro D'Andrea

## Documentación
- [Diagrama BPMN del proceso](BPMN/BPMN.png)
- [Tablero del proyecto (GitHub Projects)](https://github.com/users/Lautar055/projects/1/views/1?layout_template=board)

## Indicadores de control y estándares de desempeño

Indicadores para la auditoría técnica del sistema de inventario. Cada uno tiene una fórmula, un estándar mínimo aceptable y una frecuencia de medición.

| N.º | Indicador | Fórmula | Estándar | Frecuencia | Fuente |
|---|---|---|---|---|---|
| I-01 | Cumplimiento del plazo de implementación | Semanas reales de implementación / 8 semanas previstas | ≤ 100 % (máximo 8 semanas) | Una vez, al cierre del proyecto | Cronograma (Gantt) |
| I-02 | Cobertura de registro de equipos | Equipos registrados con número de serie / equipos en circulación × 100 | ≥ 50 % al cierre del primer año | Mensual | Base de datos interna |
| I-04 | Concordancia en auditoría | Equipos verificados que coinciden con el registro / equipos auditados × 100 | ≥ 95 % | En cada auditoría (la primera, semana 12) | Informe de auditoría |
| I-05 | Tasa de reemplazo por rotura | Equipos retirados y reemplazados por rotura en el período / equipos en circulación al inicio del período × 100 | ≤ 10 % anual | Semestral (acumulado de los últimos 12 meses) | Registro de devoluciones y base de datos interna |
| I-06 | Tiempo de atención de solicitudes | Días hábiles entre la solicitud y la entrega (con stock disponible) | ≤ 5 días hábiles | Mensual | Registro de solicitudes |

## Declaración de Uso de IA

### Herramienta utilizada
Claude (Anthropic), usado como asistente de consulta y revisión durante la Entrega N.º 4

### Prompts utilizados y justificación

| Prompt (resumen) | Para qué lo usé | Justificación |
|---|---|---|
| Pedido de ayuda con el punto 3 (Backlog Ágil), adjuntando las entregas 1, 2 y 3 y las consignas | Obtener un primer borrador de las historias de usuario y del tablero | Adjuntar las entregas anteriores evitó historias genéricas y mantuvo el caso de estudio (Escorial) y el módulo de inventario |
| "Dame las reglas para la creación del BPMN" | Repasar la notación (pools, lanes, tipos de flecha, eventos, compuertas) antes de dibujar | Asegurar el uso correcto de la notación estándar que exige la consigna |
| Consultas sobre colores y formato de exportación del diagrama | Decidir la presentación del BPMN | Resolver criterios de legibilidad: color sobrio por lane y PNG con fondo para que se vea en cualquier visor |
| "ayudame con los comandos quiero hacer lo mayor posible de esto por consola de git bash para practicar | Recibir parte de los comandos para realizar la creacion del proyecto desde la consola | Practicar el uso de los comandos en git bash en lugar de hacer la mayoria de ediciones desde el propio GitHub |
| Consultas sobre comandos de Git Bash y GitHub CLI para el flujo de ramas, commits y Pull Request | Practicar el flujo de versionado por consola | Aprender el proceso completo (rama, commit, push, PR) en lugar de usar solo la interfaz web, y poder explicarlo |
| Consulta por mensajes de advertencia y comandos | Entender qué hace cada comando antes de usarlo | Evitar subir cambios no deseados y no ejecutar comandos sin comprender su efecto |
| Pedido de indicadores de control para la auditoría del sistema | Obtener un borrador de indicadores y estándares | Partir de mis metas de la Entrega 2 y de las reglas de mi BPMN, no de indicadores genéricos |

### Correcciones humanas sobre los resultados de la IA
- Las primeras historias propuestas por la IA se derivaron del diseño de la Entrega 2 (login, auditoría, ingreso por Excel) y no coincidían con mi BPMN. Pedí rehacerlas y quedaron alineadas con los tres flujos del diagrama: solicitud/reemplazo, entrega con firma y devolución.
- No todos los comandos dados por la IA fueron necesarios, por lo que solo use los que vi necesarios
- Las decisiones finales (contenido de las historias, estructura del repositorio, diseño del BPMN) fueron mías.
- Los estándares de desempeño propuestos por la IA. Los revisé y los modifique eliminando algunos que no me parecían correctos, como un indicador que verificaba el porcentaje de entregas con firma cuando sin firma no se realiza la entrega y medicando otros como el I-05, que se mantuvo la idea general pero se aplico correctamente al programa mencionado.
