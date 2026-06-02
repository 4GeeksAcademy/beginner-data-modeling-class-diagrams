# 06 - Cuarta entidad

Version en ingles: [README.md](./README.md)

## Escenario

Los libros tienen autores. Modela la autoría como entidad propia.

## Instrucciones

1. Agrega la clase **`Author`** con:

| Propiedad | Tipo |
|-----------|------|
| `id` | `int` |
| `fullName` | `string` |
| `country` | `string` |

2. Conecta **`Author`** y **`Book`** con una relacion coherente (por ejemplo un autor escribe muchos libros, o muchos autores colaboran en muchos libros). Etiqueta la cardinalidad en ambos extremos.

## Lista de verificacion

- [ ] `Author` tiene tres propiedades tipadas.
- [ ] `Author` se relaciona con `Book` con cardinalidad clara.

## Siguiente paso

**07 - Muchos a muchos** — prestamos entre socios y libros.
