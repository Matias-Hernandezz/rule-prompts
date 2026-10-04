# FRONTEND ARCHITECTURE

## Objetivo

Construir un frontend modular, mantenible y escalable sin sobreingeniería.

---

## 1. Analizar antes de implementar

Antes de crear componentes:

* revisar estructura
* identificar rutas
* identificar componentes existentes
* identificar layouts
* identificar hooks
* identificar servicios
* identificar sistema de estilos

Reutilizar soluciones existentes cuando sea apropiado.

---

## 2. Componentes

Separar componentes cuando:

* tengan responsabilidad independiente
* sean reutilizables
* tengan lógica propia
* mejoren la legibilidad

No crear componentes innecesariamente pequeños.

Evitar:

* componentes gigantes
* componentes con múltiples responsabilidades
* lógica de negocio mezclada con presentación

---

## 3. Estado

Utilizar el nivel de estado mínimo necesario.

Preferencia:

1. estado local
2. URL
3. contexto cuando realmente corresponda
4. estado global solamente cuando exista una necesidad real

No crear un store global para problemas locales.

---

## 4. Datos

Separar:

* UI
* lógica
* acceso a API
* transformación de datos

Evitar llamadas HTTP directamente dispersas dentro de componentes visuales.

---

## 5. Tipado

Utilizar TypeScript correctamente.

Evitar:

* `any`
* casts innecesarios
* interfaces duplicadas
* tipos excesivamente complejos

Los tipos deben representar el dominio real.

---

## 6. Routing

Las rutas deben ser:

* claras
* predecibles
* consistentes

Los parámetros dinámicos deben estar correctamente tipados y validados.

---

## 7. Formularios

Los formularios deben contemplar:

* validación
* loading
* errores
* éxito
* estados vacíos
* feedback al usuario

---

## 8. Errores

No ocultar errores silenciosamente.

Mostrar mensajes útiles al usuario y mantener detalles técnicos en logs apropiados.

---

## 9. Performance

Evitar optimizaciones prematuras.

Optimizar solamente cuando:

* exista un problema
* exista un componente costoso
* haya una razón concreta

---

## 10. Regla de arquitectura

La arquitectura debe ser tan compleja como el proyecto necesita, no más.

No implementar patrones enterprise en una landing sencilla.
