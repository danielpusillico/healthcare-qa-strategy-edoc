# 04 – Test Plan (Plan de Pruebas)

## 1. Introduction (Introducción)

This test plan defines the strategy, scope, approach, resources, and schedule of testing activities for the Healthcare Appointment System.

(Este plan de pruebas define la estrategia, alcance, enfoque, recursos y cronograma de actividades de testing para el sistema de turnos médicos.)

---

## 2. Testing Objectives (Objetivos de Prueba)

- Verify that functional requirements are correctly implemented.
- Ensure system stability and reliability.
- Validate role-based access control.
- Identify defects before automation phase.

(Verificar que los requerimientos funcionales estén correctamente implementados.
Asegurar estabilidad y confiabilidad del sistema.
Validar el control de acceso por roles.
Identificar defectos antes de la fase de automatización.)

---

## 3. Testing Types (Tipos de Prueba)

The following testing types will be performed:

(Los siguientes tipos de prueba serán realizados:)

- Functional Testing
- Regression Testing
- Negative Testing
- Exploratory Testing
- Database Validation (SQL)
- Performance Testing (Phase 2)
- Security Testing (Phase 2)

---

## 4. Test Environment (Entorno de Pruebas)

- Application: eDoc Doctor Appointment System
- Environment: Local Docker setup
- Database: MySQL / MariaDB
- Browsers: Chrome (Primary)

(Aplicación: eDoc Doctor Appointment System
Entorno: Configuración local con Docker
Base de datos: MySQL / MariaDB
Navegador principal: Chrome)

---

## 5. Entry Criteria (Criterios de Entrada)

- Application deployed and accessible.
- Database configured.
- Test data available.

(Aplicación desplegada y accesible.
Base de datos configurada.
Datos de prueba disponibles.)

---

## 6. Exit Criteria (Criterios de Salida)

- All critical test cases executed.
- No high-severity defects remain unresolved.
- Test summary report completed.

(Todos los casos críticos ejecutados.
No existen defectos críticos sin resolver.
Informe final de pruebas completado.)

---

## 7. Risk Management (Gestión de Riesgos)

Potential risks include:

(Posibles riesgos incluyen:)

- Duplicate appointment booking.
- Unauthorized access to patient data.
- Session inconsistencies.
- Data integrity issues.
