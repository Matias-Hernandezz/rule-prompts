# BOOKING SYSTEM

## Objetivo

Construir un sistema de reservas confiable y fácil de utilizar.

---

## 1. Conceptos

Definir:

* usuarios
* servicios
* profesionales
* horarios
* disponibilidad
* reservas
* estados
* pagos
* notificaciones

---

## 2. Disponibilidad

La disponibilidad debe calcularse en backend.

Nunca confiar exclusivamente en el calendario del frontend.

---

## 3. Reservas

Una reserva debe contemplar:

* usuario
* servicio
* profesional cuando corresponda
* fecha
* horario
* estado
* timestamps

---

## 4. Concurrencia

Prevenir:

* doble reserva
* doble confirmación
* reservas simultáneas

El backend debe validar nuevamente la disponibilidad antes de confirmar.

---

## 5. Estados

Definir estados explícitos.

Ejemplo:

* pending
* confirmed
* cancelled
* completed
* no_show

No utilizar strings arbitrarios por todo el proyecto.

---

## 6. Cancelaciones

Definir claramente:

* cuándo puede cancelar
* qué sucede con el horario
* qué sucede con el pago
* qué sucede con el depósito

---

## 7. Pagos

Cuando exista seña:

* validar pago
* registrar estado
* asociar pago con reserva
* procesar webhooks
* evitar duplicados

---

## 8. Notificaciones

Contemplar:

* confirmación
* recordatorio
* cancelación
* cambios

No bloquear la reserva si un sistema externo de notificaciones falla, salvo que sea una regla explícita del negocio.

---

## 9. UX

El usuario debe poder entender:

* qué servicio está reservando
* duración
* precio
* profesional
* fecha
* horario
* estado

---

## 10. Admin

El administrador debería poder gestionar:

* horarios
* bloqueos
* reservas
* clientes
* cambios
* métricas relevantes

---

## 11. Integridad

El backend debe proteger contra:

* doble reserva
* horarios inválidos
* servicios inexistentes
* usuarios inexistentes
* modificaciones no autorizadas

---

## 12. Regla

La disponibilidad real siempre pertenece al backend.
