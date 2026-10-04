# DATABASE DESIGN

## Objetivo

Diseñar una base de datos consistente, clara y preparada para el crecimiento real del proyecto.

---

## 1. Analizar dominio

Antes de crear tablas:

Identificar:

* entidades
* relaciones
* atributos
* reglas de negocio
* restricciones
* cardinalidades

No crear tablas basándose únicamente en cómo se ve la interfaz.

---

## 2. Normalización

Evitar duplicación innecesaria.

Normalizar cuando mejore:

* consistencia
* mantenimiento
* integridad

No sobre-normalizar si genera complejidad innecesaria.

---

## 3. Primary keys

Cada entidad persistente debe tener una identificación estable.

---

## 4. Foreign keys

Utilizar relaciones explícitas.

Definir comportamiento ante:

* delete
* update
* registros relacionados

---

## 5. Constraints

Cuando corresponda utilizar:

* NOT NULL
* UNIQUE
* CHECK
* FOREIGN KEY

Las reglas importantes deben existir también en la base de datos, no únicamente en la aplicación.

---

## 6. Índices

Crear índices para consultas frecuentes.

No indexar absolutamente todo.

Considerar:

* filtros
* joins
* búsquedas
* ordenamientos

---

## 7. Migraciones

Nunca modificar producción manualmente si el proyecto utiliza migraciones.

Toda modificación estructural debe poder reproducirse.

---

## 8. Integridad

La base de datos debe impedir estados inválidos cuando sea posible.

---

## 9. Performance

Analizar consultas antes de introducir optimizaciones complejas.

---

## 10. Regla principal

La estructura de la base de datos debe representar el dominio del negocio, no solamente la estructura actual del frontend.
