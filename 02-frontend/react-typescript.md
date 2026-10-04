# REACT + TYPESCRIPT

## Principios

Utilizar React y TypeScript siguiendo patrones simples y mantenibles.

---

## Componentes

Preferir componentes funcionales.

Cada componente debe tener una responsabilidad clara.

Utilizar props tipadas explícitamente.

---

## Props

Crear interfaces/types cuando aporten claridad.

Evitar props innecesarias.

Si un componente recibe demasiadas props, evaluar dividir responsabilidades.

---

## Hooks

Crear hooks personalizados cuando exista lógica reutilizable.

No crear hooks simplemente para mover unas pocas líneas.

---

## Estado

Mantener el estado lo más cerca posible de donde se utiliza.

Evitar prop drilling excesivo.

---

## Efectos

No utilizar `useEffect` para lógica que puede resolverse directamente durante el renderizado o mediante eventos.

Cada efecto debe tener un motivo claro.

---

## Listas

Utilizar keys estables.

Nunca utilizar índices como key cuando los elementos puedan cambiar de posición.

---

## TypeScript

Evitar `any`.

Preferir tipos específicos.

No utilizar `as` para ocultar errores de tipado salvo que exista una razón válida.

---

## Código

Priorizar:

* legibilidad
* simplicidad
* composición
* reutilización razonable

Evitar abstracciones prematuras.
