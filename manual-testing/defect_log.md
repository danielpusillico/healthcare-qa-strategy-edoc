# Defect Log (Registro de Defectos)

This document contains identified defects during manual testing execution.

(Este documento contiene los defectos identificados durante la ejecución de pruebas manuales.)

---

## Defect Severity Legend (Severidad)

- Critical – System unusable / data loss (Sistema inutilizable / pérdida de datos)
- High – Major functionality broken (Funcionalidad principal afectada)
- Medium – Partial functionality issue (Problema parcial)
- Low – Cosmetic / minor issue (Problema menor / visual)

---

## DEF-001 – Duplicate Appointment Allowed

- **Module**: Appointment Booking
- **Severity**: High
- **Priority**: P1
- **Environment**: Local Docker
- **Steps to Reproduce**:
  1. Login as Patient
  2. Book an available appointment
  3. Attempt to book the same slot again
- **Expected Result**:
  System should prevent duplicate booking.
- **Actual Result**:
  System allows booking the same slot twice.
- **Status**: Open

---

## DEF-002 – Access Control Bypass via Direct URL

- **Module**: Role-Based Access
- **Severity**: Critical
- **Priority**: P1
- **Environment**: Local Docker
- **Steps to Reproduce**:
  1. Login as Patient
  2. Manually enter Admin-only URL in browser
- **Expected Result**:
  Access denied or redirect to unauthorized page.
- **Actual Result**:
  Page loads without proper restriction.
- **Status**: Open

---

## DEF-003 – Missing Validation for Past Date Booking

- **Module**: Appointment Booking
- **Severity**: High
- **Priority**: P1
- **Steps to Reproduce**:
  1. Login as Patient
  2. Select past date for booking
  3. Confirm
- **Expected Result**:
  System blocks booking.
- **Actual Result**:
  Booking is created.
- **Status**: Open

---

## DEF-004 – Session Overlap Not Blocked

- **Module**: Session Management
- **Severity**: High
- **Priority**: P2
- **Steps to Reproduce**:
  1. Login as Admin
  2. Create session for Doctor at 10:00 AM
  3. Create another session at same time
- **Expected Result**:
  System prevents overlapping sessions.
- **Actual Result**:
  System allows overlap.
- **Status**: Open

---

## DEF-005 – UI Alignment Issue on Dashboard

- **Module**: Dashboard
- **Severity**: Low
- **Priority**: P3
- **Steps to Reproduce**:
  1. Login as Doctor
  2. View dashboard
- **Expected Result**:
  Proper UI alignment.
- **Actual Result**:
  Misaligned button in header.
- **Status**: Open
