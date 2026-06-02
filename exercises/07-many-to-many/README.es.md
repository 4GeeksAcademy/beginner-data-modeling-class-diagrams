# 07 - Muchos a muchos

Version en ingles: [README.md](./README.md)

## Escenario

Un socio puede pedir muchos libros en el tiempo y un libro puede ser prestado por muchos socios (en fechas distintas). Modela ese patron **muchos a muchos** con una clase de asociacion.

## Instrucciones

1. Agrega la clase **`Loan`** (asociacion) con al menos:

| Propiedad | Tipo |
|-----------|------|
| `id` | `int` |

2. Enlaza **`Member`** y **`Book`** mediante **`Loan`** para una relacion **muchos a muchos (N:M)**:
   - Un socio puede tener muchos prestamos.
   - Un libro puede aparecer en muchos prestamos.

3. Etiqueta cardinalidades en las rutas `Member` — `Loan` — `Book`.

## Lista de verificacion

- [ ] `Loan` existe entre `Member` y `Book`.
- [ ] La cardinalidad refleja historial de prestamos **N:M**.

## Siguiente paso

**08 - Repaso de propiedades tipadas** — fechas en `Loan`.
