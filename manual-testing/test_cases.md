# Test Cases (Casos de Prueba)

## Legend (Leyenda)
- **Priority**: P1 (High), P2 (Medium), P3 (Low)  
  (Prioridad: P1 Alta, P2 Media, P3 Baja)
- **Type**: Functional / Negative / Regression / Smoke  
  (Tipo: Funcional / Negativa / Regresión / Smoke)
- **Roles**: Admin / Doctor / Patient  
  (Roles: Administrador / Médico / Paciente)

---

## Authentication (Autenticación)

### TC-AUTH-001 – Valid Login (Inicio de sesión válido)
- **Role**: Patient (Paciente)
- **Priority**: P1
- **Type**: Smoke, Functional
- **Preconditions (Precondiciones)**: User account exists (Existe cuenta de usuario)
- **Steps (Pasos)**:
  1. Navigate to Login page (Ir a la página de login)
  2. Enter valid email and password (Ingresar email y password válidos)
  3. Click "Login" (Click en "Login")
- **Expected Result (Resultado esperado)**:
  - User is redirected to dashboard/home (Redirige al panel/inicio)

### TC-AUTH-002 – Invalid Login (Inicio de sesión inválido)
- **Role**: Patient (Paciente)
- **Priority**: P1
- **Type**: Negative
- **Preconditions**: None (Ninguna)
- **Steps**:
  1. Navigate to Login page
  2. Enter invalid email/password
  3. Click "Login"
- **Expected Result**:
  - Error message is displayed and login is denied
  (Se muestra mensaje de error y se bloquea el login)

### TC-AUTH-003 – Role Access Restriction (Restricción por rol)
- **Role**: Patient (Paciente)
- **Priority**: P1
- **Type**: Functional, Security
- **Preconditions**: Patient is logged in (Paciente logueado)
- **Steps**:
  1. Try to access an Admin-only URL directly (Intentar acceder a URL solo Admin)
- **Expected Result**:
  - Access is denied or redirected to login/unauthorized page
  (Acceso denegado o redirige a login/no autorizado)

---

## Patient Registration (Registro de Paciente)

### TC-REG-001 – Register with valid data (Registro con datos válidos)
- **Role**: Patient (Paciente)
- **Priority**: P1
- **Type**: Functional
- **Preconditions**: Email not used (Email no registrado)
- **Steps**:
  1. Navigate to patient registration page
  2. Fill mandatory fields with valid values
  3. Submit registration
- **Expected Result**:
  - Patient account is created successfully
  (Cuenta creada correctamente)

### TC-REG-002 – Register with invalid email format (Email inválido)
- **Role**: Patient
- **Priority**: P2
- **Type**: Negative
- **Preconditions**: None
- **Steps**:
  1. Navigate to registration page
  2. Enter invalid email (e.g., "user@")
  3. Submit
- **Expected Result**:
  - Validation error is shown; user is not created
  (Se muestra error; no se crea usuario)

---

## Appointment Booking (Reserva de Turno)

### TC-APPT-001 – Book an available appointment (Reservar turno disponible)
- **Role**: Patient
- **Priority**: P1
- **Type**: Smoke, Functional
- **Preconditions**:
  - Patient logged in
  - At least one doctor session exists
  (Paciente logueado y existe una sesión médica)
- **Steps**:
  1. Navigate to booking module
  2. Select a doctor/session
  3. Confirm booking
- **Expected Result**:
  - Appointment is created and visible in "My Appointments"
  (Turno creado y visible en "Mis turnos")

### TC-APPT-002 – Prevent past date booking (Evitar fecha pasada)
- **Role**: Patient
- **Priority**: P1
- **Type**: Negative, Regression
- **Preconditions**: Patient logged in
- **Steps**:
  1. Navigate to booking
  2. Attempt to select a past date/session
  3. Submit
- **Expected Result**:
  - System blocks booking and shows validation message
  (Bloquea la reserva y muestra validación)

### TC-APPT-003 – Cancel appointment (Cancelar turno)
- **Role**: Patient
- **Priority**: P1
- **Type**: Functional, Regression
- **Preconditions**: Patient has an existing appointment (Paciente con turno existente)
- **Steps**:
  1. Go to "My Appointments"
  2. Select an appointment
  3. Click "Cancel"
- **Expected Result**:
  - Appointment status changes to Cancelled and is no longer active
  (Estado cambia a Cancelado y no queda activo)

---

## Admin – Session Management (Admin – Gestión de Sesiones)

### TC-ADMIN-001 – Create doctor session (Crear sesión médica)
- **Role**: Admin
- **Priority**: P1
- **Type**: Functional
- **Preconditions**: Admin logged in (Admin logueado)
- **Steps**:
  1. Navigate to session management
  2. Create a session with valid doctor + date/time
  3. Save
- **Expected Result**:
  - Session is created and visible in session list
  (Sesión creada y visible en listado)

### TC-ADMIN-002 – Prevent overlapping sessions (Evitar sesiones superpuestas)
- **Role**: Admin
- **Priority**: P1
- **Type**: Negative
- **Preconditions**: Existing session for same doctor/time
- **Steps**:
  1. Attempt to create a new session overlapping an existing one
  2. Save
- **Expected Result**:
  - System blocks overlap or warns appropriately
  (Bloquea superposición o avisa)

---

## Doctor – View Schedule (Médico – Ver Agenda)

### TC-DOC-001 – View assigned appointments (Ver turnos asignados)
- **Role**: Doctor
- **Priority**: P1
- **Type**: Functional
- **Preconditions**: Doctor logged in; appointments exist
- **Steps**:
  1. Login as Doctor
  2. Navigate to schedule/appointments view
- **Expected Result**:
  - Doctor sees list of upcoming appointments
  (Ve listado de turnos próximos)
