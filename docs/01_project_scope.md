# 01 – Project Scope (Alcance del Proyecto)

## 1. System Overview (Descripción del Sistema)

The system under test is the eDoc Doctor Appointment Management System, a web-based healthcare application designed to manage patient appointments, doctor schedules, and administrative operations.

(El sistema bajo prueba es eDoc Doctor Appointment Management System, una aplicación web de salud diseñada para gestionar turnos de pacientes, agendas médicas y operaciones administrativas.)

---

## 2. Objective of Testing (Objetivo del Testing)

The objective of this QA strategy is to validate that the system functions correctly, securely, and reliably under expected conditions, ensuring data integrity and proper role-based access control.

(El objetivo de esta estrategia de QA es validar que el sistema funcione correctamente, de forma segura y confiable bajo condiciones esperadas, asegurando la integridad de los datos y el control de acceso por roles.)

---

## 3. Modules in Scope (Módulos Incluidos)

The following modules are included in this testing scope:

(Los siguientes módulos están incluidos en el alcance de pruebas:)

- Authentication (Admin / Doctor / Patient)
  (Autenticación – Administrador / Médico / Paciente)

- Appointment Booking
  (Reserva de turnos)

- Session Management
  (Gestión de sesiones médicas)

- Role-Based Access Control
  (Control de acceso basado en roles)

- Patient Management
  (Gestión de pacientes)

---

## 4. Modules Out of Scope (Módulos Fuera de Alcance)

The following areas are not included in this testing phase:

(Las siguientes áreas no están incluidas en esta fase de pruebas:)

- Payment processing
  (Procesamiento de pagos)

- External integrations
  (Integraciones externas)

- Third-party services
  (Servicios de terceros)

---

## 5. Testing Approach Overview (Resumen del Enfoque de Testing)

The testing strategy will include:

(La estrategia de pruebas incluirá:)

- Functional Testing
  (Pruebas funcionales)

- Regression Testing
  (Pruebas de regresión)

- Negative Testing
  (Pruebas negativas)

- Exploratory Testing
  (Pruebas exploratorias)

- UI Automation (Cypress – Phase 2)
  (Automatización de interfaz – Fase 2)

- API Testing (Postman – Phase 3)
  (Pruebas de API – Fase 3)

- Database Validation (SQL queries)
  (Validación de base de datos mediante consultas SQL)

---

## 6. Risk Considerations (Consideraciones de Riesgo)

Due to the healthcare nature of the system, particular attention will be given to:

(Debido a la naturaleza de salud del sistema, se prestará especial atención a:)

- Data integrity
  (Integridad de los datos)

- Access control enforcement
  (Control de acceso)

- Session consistency
  (Consistencia de sesión)

- Appointment duplication prevention
  (Prevención de duplicación de turnos)

---

## 7. Environment (Entorno)

Testing will be performed in a local Docker-based environment replicating a development setup.

(Las pruebas se realizarán en un entorno local basado en Docker que replica un entorno de desarrollo.)
