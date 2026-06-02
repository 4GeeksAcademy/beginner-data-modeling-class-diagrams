# 08 - Repaso de propiedades tipadas

Version en ingles: [README.md](./README.md)

## Escenario

Cada prestamo registra cuando se entrego el libro y cuando debe devolverse.

## Instrucciones

Amplía **`Loan`** con:

| Propiedad | Tipo |
|-----------|------|
| `loanDate` | `date` |
| `dueDate` | `date` |

Revisa el diagrama y confirma que usas estos tipos de forma coherente:

- `int` — identificadores y conteos
- `string` — nombres, codigos, email
- `boolean` — banderas como `isAvailable`
- `date` — campos de calendario como `issuedAt`, `loanDate`, `dueDate`

## Lista de verificacion

- [ ] `Loan` incluye las dos propiedades `date`.
- [ ] Al menos cuatro clases distintas siguen en el lienzo.
- [ ] Cada propiedad del diagrama muestra un tipo explicito.

## Siguiente paso

**09 - Modelo completo** — pulir el diagrama de la biblioteca.
