```markdown
# Requerimientos y Backlog: HealthTrack Connect

**Link al Tablero de Gestión:** [https://github.com/users/Cesar9574/projects/1/views/2]

## 1. Historias de Usuario (Backlog)

| ID | Historia de Usuario | Prioridad |
| :--- | :--- | :--- |
| HU01 | Como paciente, quiero ver los horarios disponibles de un médico para elegir uno. | **Must** |
| HU02 | Como administrador, quiero crear perfiles de médicos para organizar la oferta. | **Must** |
| HU03 | Como paciente, quiero cancelar mi cita con antelación para liberar el cupo. | Should |
| HU04 | Como médico, quiero ver mi agenda del día para prepararme para las consultas. | Should |
| HU05 | Como paciente, quiero recibir un correo de confirmación al agendar una cita. | Could |
| HU06 | Como administrador, quiero exportar la lista de pacientes a Excel. | Could |
| HU07 | Como paciente, quiero subir una foto de mi orden médica previa. | Could |
| HU08 | Como médico, quiero recetar medicamentos digitalmente (Firma electrónica). | Won't |

## 2. Criterios de Aceptación (Historias Críticas)

### HU01: Ver horarios disponibles (Formato Given/When/Then)
* **Given:** El paciente ha seleccionado la especialidad de "Medicina General".
* **When:** Hace clic en el calendario de un médico específico.
* **Then:** El sistema debe mostrar únicamente los bloques de tiempo que no estén ocupados por otras citas confirmadas.

### HU02: Crear perfiles médicos (Formato Given/When/Then)
* **Given:** El administrador ha iniciado sesión en el panel de configuración.
* **When:** Completa el formulario con nombre, especialidad y número de colegiado.
* **Then:** El sistema debe guardar el perfil y habilitar el calendario de ese médico para recibir citas.

## 3. MVP Rationale
Para el lanzamiento inicial de **HealthTrack Connect**, hemos priorizado las historias **HU01** y **HU02** como **Must**. La razón es que estas constituyen el núcleo transaccional: sin médicos registrados y sin visualización de disponibilidad, el sistema no tiene funcionalidad básica. El enfoque del MVP es validar el flujo de agendamiento antes de añadir complejidad administrativa.
