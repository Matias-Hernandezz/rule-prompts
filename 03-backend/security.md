# SECURITY

## Principio

Toda entrada proveniente del usuario debe considerarse potencialmente maliciosa.

---

## Autenticación

Nunca almacenar contraseñas en texto plano.

Utilizar mecanismos de hashing adecuados.

---

## Autorización

Verificar permisos en backend.

No depender de:

* botones ocultos
* rutas ocultas
* validaciones frontend

---

## Secrets

Nunca colocar en:

* código fuente
* frontend
* commits
* archivos públicos

secretos como:

* API keys
* passwords
* tokens
* private keys

---

## SQL

Utilizar queries parametrizadas o mecanismos ORM seguros.

Nunca construir SQL utilizando concatenación directa de input del usuario.

---

## XSS

Sanitizar contenido cuando sea necesario.

No utilizar HTML arbitrario sin una razón clara.

---

## CORS

Configurar CORS explícitamente.

No utilizar `*` indiscriminadamente en producción.

---

## Rate limiting

Considerarlo para:

* login
* recuperación de contraseña
* endpoints públicos
* APIs costosas

---

## Uploads

Validar:

* tamaño
* extensión
* MIME type
* nombre
* almacenamiento

No confiar únicamente en la extensión.

---

## Errores

Nunca exponer información interna del servidor al usuario final.

---

## Dependencias

Evitar dependencias innecesarias.

Mantenerlas actualizadas cuando corresponda.

---

## Regla final

La seguridad debe implementarse en backend incluso si el frontend ya valida los datos.
