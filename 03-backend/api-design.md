# API DESIGN

## REST

Cuando se utilice REST:

* utilizar recursos claros
* utilizar métodos HTTP apropiados
* mantener respuestas consistentes
* utilizar códigos HTTP correctos

Ejemplo conceptual:

GET /products

GET /products/{id}

POST /products

PUT/PATCH /products/{id}

DELETE /products/{id}

---

## Respuestas

Mantener estructuras consistentes.

Errores:

* código
* mensaje
* detalles cuando corresponda

---

## Validación

Toda entrada externa debe considerarse no confiable.

Validar en backend.

---

## Paginación

Para colecciones potencialmente grandes utilizar paginación.

No devolver miles de registros innecesariamente.

---

## Filtros

Los filtros deben ser explícitos y predecibles.

---

## Autorización

Cada endpoint protegido debe verificar permisos.

No confiar en el frontend.

---

## Versionado

Implementar versionado cuando el proyecto realmente lo requiera.

No introducir versionado innecesariamente en proyectos pequeños.

---

## Documentación

Mantener documentación de endpoints importantes.

Describir:

* parámetros
* request
* response
* errores
* autenticación
