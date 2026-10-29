# Sistema de Inventario de Equipos - Escorial

## Descripción
Sistema de información para controlar la entrega, devolución y reemplazo de equipos de sistemas (PC, teclados, monitores, etc.) entregados a los empleados de Escorial, relacionando cada elemento con su número de serie y con el empleado a cargo.

Proyecto de la materia Organización Empresarial, Tecnicatura Universitaria en Programación (UTN).

## Integrantes
- Lautaro D'Andrea

## Documentación
- [Diagrama BPMN del proceso](BPMN/BPMN.png)
- [Tablero del proyecto (GitHub Projects)](https://github.com/users/Lautar055/projects/1/views/1?layout_template=board)

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

### Correcciones humanas sobre los resultados de la IA
- Las primeras historias propuestas por la IA se derivaron del diseño de la Entrega 2 (login, auditoría, ingreso por Excel) y no coincidían con mi BPMN. Pedí rehacerlas y quedaron alineadas con los tres flujos del diagrama: solicitud/reemplazo, entrega con firma y devolución.
- No todos los comandos dados por la IA fueron necesarios, por lo que solo use los que vi necesarios
- Las decisiones finales (contenido de las historias, estructura del repositorio, diseño del BPMN) fueron mías.
