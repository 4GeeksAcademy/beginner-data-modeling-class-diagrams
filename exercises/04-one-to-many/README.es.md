# 04 - Uno a muchos

Version en ingles: [README.md](./README.md)

## Escenario

La biblioteca tiene varias sucursales. Cada sucursal almacena muchos libros, pero cada libro esta en una sucursal.

## Instrucciones

1. Agrega la clase **`Branch`** con:

| Propiedad | Tipo |
|-----------|------|
| `id` | `int` |
| `name` | `string` |
| `city` | `string` |

2. Dibuja una relacion **uno a muchos (1:N)**: una **`Branch`** tiene muchos **`Book`**.
3. Etiqueta la cardinalidad en ambos extremos (por ejemplo `1` en sucursal y `N` o `*` en libro).

## Lista de verificacion

- [ ] `Branch` esta modelada con propiedades tipadas.
- [ ] Cada `Book` se vincula a exactamente una `Branch` en tu diagrama.

## Siguiente paso

**05 - Propiedad booleana** — disponibilidad del libro.
