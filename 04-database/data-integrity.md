# DATA INTEGRITY

## Objetivo

Garantizar que el sistema no pueda generar estados de datos inválidos.

---

## Reglas

Identificar explícitamente:

* valores obligatorios
* valores únicos
* relaciones
* estados
* transiciones
* límites
* condiciones especiales

---

## Transacciones

Cuando una operación involucre múltiples cambios dependientes, evaluar si debe ejecutarse dentro de una transacción.

---

## Concurrencia

Para operaciones sensibles considerar:

* race conditions
* doble reserva
* doble pago
* stock negativo
* actualizaciones simultáneas

---

## Idempotencia

Para operaciones que puedan repetirse:

* pagos
* webhooks
* reservas
* emails
* tareas automáticas

considerar mecanismos de idempotencia.

---

## Estados

Definir estados válidos explícitamente.

Evitar strings arbitrarios dispersos por el código.

---

## Regla

El sistema debe proteger la integridad de los datos incluso cuando:

* el frontend falla
* el usuario manipula requests
* una request se repite
* dos usuarios realizan acciones simultáneamente
