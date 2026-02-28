# 02 – Functional Requirements (Requerimientos Funcionales)

## 1. User Authentication (Autenticación de Usuarios)

FR-01: The system shall allow users (Admin, Doctor, Patient) to log in using valid credentials.
(El sistema deberá permitir a los usuarios iniciar sesión con credenciales válidas.)

FR-02: The system shall prevent login with invalid credentials.
(El sistema deberá impedir el inicio de sesión con credenciales inválidas.)

FR-03: The system shall restrict access to features based on user roles.
(El sistema deberá restringir el acceso a funcionalidades según el rol del usuario.)

FR-04: The system shall terminate user sessions after logout.
(El sistema deberá finalizar la sesión del usuario al cerrar sesión.)

---

## 2. Patient Registration (Registro de Pacientes)

FR-05: The system shall allow new patients to register with mandatory fields.
(El sistema deberá permitir registrar nuevos pacientes con campos obligatorios.)

FR-06: The system shall validate email format during registration.
(El sistema deberá validar el formato del correo electrónico durante el registro.)

FR-07: The system shall prevent duplicate patient accounts using the same email.
(El sistema deberá impedir cuentas duplicadas con el mismo correo electrónico.)

---

## 3. Appointment Booking (Reserva de Turnos)

FR-08: The system shall allow patients to view available doctor sessions.
(El sistema deberá permitir a los pacientes visualizar sesiones médicas disponibles.)

FR-09: The system shall allow patients to book an available appointment slot.
(El sistema deberá permitir reservar un turno disponible.)

FR-10: The system shall prevent booking appointments in past dates.
(El sistema deberá impedir reservar turnos en fechas pasadas.)

FR-11: The system shall prevent double booking for the same time slot.
(El sistema deberá impedir la reserva doble para el mismo horario.)

FR-12: The system shall display confirmation after successful booking.
(El sistema deberá mostrar confirmación luego de una reserva exitosa.)

---

## 4. Doctor Session Management (Gestión de Sesiones Médicas)

FR-13: Admin shall be able to create new doctor sessions.
(El administrador deberá poder crear nuevas sesiones médicas.)

FR-14: Admin shall be able to edit existing sessions.
(El administrador deberá poder editar sesiones existentes.)

FR-15: Admin shall be able to delete sessions.
(El administrador deberá poder eliminar sesiones.)

FR-16: The system shall prevent overlapping sessions for the same doctor.
(El sistema deberá impedir sesiones superpuestas para el mismo médico.)

---

## 5. Appointment Management (Gestión de Turnos)

FR-17: Patients shall be able to view their booked appointments.
(Los pacientes deberán poder visualizar sus turnos reservados.)

FR-18: Patients shall be able to cancel appointments.
(Los pacientes deberán poder cancelar turnos.)

FR-19: Doctors shall be able to view their scheduled appointments.
(Los médicos deberán poder visualizar sus turnos asignados.)

FR-20: The system shall update appointment status after cancellation.
(El sistema deberá actualizar el estado del turno luego de una cancelación.)
