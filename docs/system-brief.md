# System Brief: HealthTrack Connect

## 1. Problema
Los consultorios médicos pequeños pierden ingresos y eficiencia debido al uso de agendas físicas (papel), lo que provoca citas duplicadas, olvidos por parte de los pacientes y falta de historial de asistencia.

## 2. Stakeholders
* **Pacientes:** Usuarios que consultan disponibilidad y reservan citas.
* **Médicos:** Profesionales que gestionan su horario y consultan su agenda diaria.
* **Administrador de Clínica:** Encargado de gestionar el catálogo de médicos y especialidades.

## 3. Scope (Alcance)
* Registro de perfiles médicos y especialidades.
* Calendario de disponibilidad en tiempo real.
* Sistema de reserva de citas para pacientes.
* Panel de visualización de agenda para el médico.

## 4. No-Scope (Fuera de Alcance)
* Procesamiento de pagos de consultas.
* Generación de recetas médicas digitales con firma electrónica.
* Consultas por videollamada (Telemedicina).

## 5. Diagrama de Contexto
```mermaid
graph LR
    P[Paciente] -- Agenda cita --> S[HealthTrack Connect]
    M[Médico] -- Define Horarios --> S
    S -- Envía Notificación --> E[Servicio Email]
    S -- Consulta/Guarda --> DB[(Base de Datos)]
