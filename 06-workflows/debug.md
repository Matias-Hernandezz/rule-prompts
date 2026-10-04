# DEBUGGING

## Objetivo

Encontrar la causa real del problema en lugar de aplicar parches.

---

## Proceso

### 1. Reproducir

Determinar:

* qué sucede
* cuándo sucede
* cómo reproducirlo

### 2. Identificar

Analizar:

* logs
* errores
* stack trace
* requests
* responses
* estado

### 3. Hipótesis

Proponer posibles causas.

### 4. Verificar

Comprobar las hipótesis antes de modificar código.

### 5. Corregir

Aplicar la solución mínima correcta.

### 6. Verificar

Comprobar:

* problema original
* casos relacionados
* regresiones

---

## Evitar

No solucionar errores mediante:

* try/catch que oculten el problema
* desactivar validaciones
* eliminar funcionalidades
* hardcodear resultados
* ignorar warnings

---

## Regla

Corregir la causa raíz, no solamente el síntoma.
