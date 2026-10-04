# REFACTOR

## Objetivo

Mejorar estructura y mantenibilidad sin cambiar comportamiento.

---

## Antes

Identificar:

* duplicación
* complejidad
* acoplamiento
* componentes gigantes
* funciones largas
* dependencias innecesarias

---

## Regla principal

El comportamiento existente debe mantenerse salvo que el objetivo del refactor indique explícitamente lo contrario.

---

## No hacer

* reescribir todo
* cambiar stack
* introducir patrones innecesarios
* modificar APIs sin necesidad
* cambiar database sin necesidad

---

## Proceso

1. Analizar.
2. Identificar problemas.
3. Proponer estrategia.
4. Implementar pequeños cambios.
5. Verificar.
6. Continuar.

---

## Resultado

El código final debe ser:

* más claro
* más modular
* igual de funcional
* más fácil de mantener
