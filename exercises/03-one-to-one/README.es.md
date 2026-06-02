# 03 - Uno a uno

Version en ingles: [README.md](./README.md)

## Escenario

Cada socio tiene exactamente un carnet de biblioteca y cada carnet pertenece a un solo socio.

## Instrucciones

1. Agrega la clase **`LibraryCard`** con:

| Propiedad | Tipo |
|-----------|------|
| `id` | `int` |
| `cardNumber` | `string` |
| `issuedAt` | `date` |

2. Dibuja una relacion **uno a uno (1:1)** entre **`Member`** y **`LibraryCard`**.
3. Etiqueta los extremos para dejar claro que cada socio tiene un carnet y cada carnet pertenece a un socio.

## Lista de verificacion

- [ ] `LibraryCard` existe con propiedades tipadas.
- [ ] La cardinalidad muestra **1:1** entre `Member` y `LibraryCard`.

## Siguiente paso

**04 - Uno a muchos** — los libros perteneceran a sucursales.
