# SAAS

## Objetivo

Construir una aplicación SaaS preparada para múltiples usuarios y crecimiento progresivo.

---

## Multi-tenancy

Determinar explícitamente si el sistema utilizará:

* tenant por usuario
* tenant por organización
* base compartida
* separación por schema
* separación por database

No asumir una estrategia sin analizar el proyecto.

---

## Usuarios

Definir:

* autenticación
* roles
* permisos
* organizaciones
* membresías

---

## Autorización

No asumir que un usuario autenticado puede acceder a todos los recursos.

Cada recurso debe verificar ownership o permisos.

---

## Billing

Separar:

* usuario
* suscripción
* plan
* estado de pago
* facturación

---

## Planes

Definir claramente:

* límites
* features
* acceso
* estado

No depender exclusivamente del frontend para imponer límites.

---

## Backend

Las reglas críticas deben implementarse en backend.

---

## Database

Las relaciones deben contemplar correctamente:

tenant → users → resources

Evitar fugas de información entre tenants.

---

## Seguridad

Una consulta nunca debería devolver recursos pertenecientes a otro tenant.

---

## Escalabilidad

No implementar infraestructura compleja prematuramente.

Diseñar para poder evolucionar.

---

## UX

El usuario debe entender:

* qué plan tiene
* qué puede utilizar
* qué límites posee
* cuándo se renueva
* qué sucede si supera un límite
